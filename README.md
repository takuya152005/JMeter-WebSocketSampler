JMeter
======

JMeter - WebSocket Sampler with Ping Support.

This based on a modified (by https://github.com/johannest) version of maciejzaleski/JMeter-WebSocketSampler that takes in the changes to thread pooling and cookie handling from tradingscreen/JMeter-WebSocketSampler and has a Ping support.

Improvements made by me for better Vaadin Push testing:
- sending one web socket message per WebSocketSampler component without pause and close "tags"
- saving raw response
- reaching timeout is now recognized as error
- new preProcessMessage and postProcessMessage methods for adding / escaping message length to/from message content (required by Atmosphere)
- resources (executors) clearing when test ends
- "Clear backlog" property is by default set to true
- some bug fixes suggested by FindBugs