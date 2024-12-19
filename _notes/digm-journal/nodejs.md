Let's make our yellowtail app collaborative so that people can interact online!

Some notes from node.js:
- Automatically generating package.json file for dependencies
- Separating client-side files in a folder
- Using web sockets to send messages between client and server

For yellowtail:
- When a person draws a line, on pointerup, send the list of paths to the server
- Callbacks/event listeners to run code whenever new messages are received/when new clients connect to the server
	- 