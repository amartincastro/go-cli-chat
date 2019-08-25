# go-cli-chat
CLI Chat Server

To run:
- go run main.go

To connect clients:
- telnet localhost 3333 (port can be edited in config.json)

This CLI application is a chat server written in Go that meets the following criteria:
- Multiple clients can connect to the server using Telnet
- Clients are asked to enter their name upon server connection
- Messages sent to the server are relayed to all connected clients
- Messages sent to the server contain client name and timestamp
- All messages are logged to a local log file
- Basic configuration settings like listening port, IP, and log file location are read from a local configuration file

Resources: 
- Main chat functionality: https://rosettacode.org/wiki/Chat_server#Go 
- Configuration file functionality: https://github.com/jamischarles/go-chat-server/blob/master/main.go 
- Logging functionality: https://stackoverflow.com/a/51628140
