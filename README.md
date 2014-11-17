# Chat
Implement the necessary methods to have a working chat room.

## Server interaction
There are 2 ways of interaction the chat server. You sending messages or recieving messages. The way you send messages is visa the `socket.emit` function. You listen, *or recieve*, for messages via `socket.on` function.

### Format
- `socket.emit('event_name', msg)`
- `socket.on('event_name', callback)`

### Input events
These are the events that you *the clients* can send **to the server**.

- `sendMsg` tells the server you want to send a message to the chat

### Outgoing
These events the server will **send to you**.

- `msg` This is the server sending you a new message.

## Steps to get chat working
### Function 1
- Onclicking the 'send' button get the text from the input field
- Clear the text from the field
- send the `sendMsg` to the server and include the chat message

### Function 2
- Listen for the `msg` event
- add the message to the message list