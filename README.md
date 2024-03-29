# go-cli-chat
## CLI Chat Server

### To run:
- go run main.go

### To connect clients:
- telnet localhost 3333 (port can be edited in config.json)

### Software Requirements:
- Multiple clients can connect to the server using Telnet
- Clients are asked to enter their name upon server connection
- Messages sent to the server are relayed to all connected clients
- Messages sent to the server contain client name and timestamp
- All messages are logged to a local log file
- Basic configuration settings like listening port, IP, and log file location are read from a local configuration file

### Resources & 3rd party code used: 
- Main chat functionality: https://rosettacode.org/wiki/Chat_server#Go 
- Configuration file functionality: https://github.com/jamischarles/go-chat-server/blob/master/main.go 
- Logging functionality: https://stackoverflow.com/a/51628140
- Words of encouragement: Joel Guerra, Seth Voltz

### Known Bugs
- Port blocking on Windows computers can prevent the application from being run twice in a row. Can be circumvented by editing the port in config.json on every subsequent run of the application
- Messages sent to the server duplicate based on number of clients connected
- Backspaces and enters used in CLI requests sent to the server show up in chat relay and logs as unescaped characters. Future releases escape characters to avoid unintended messages and potential vulnerabilities
