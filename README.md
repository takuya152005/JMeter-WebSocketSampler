JMeter
======

JMeter - WebSocket Sampler with Ping Support.

This based on a modified (by https://github.com/ramsperger) version of maciejzaleski/JMeter-WebSocketSampler that takes in the changes to thread pooling and cookie handling from tradingscreen/JMeter-WebSocketSampler and has a Ping support.

Modified further by me to enable sending several frames in a WebSocketSampler with pauses between them to make it more easy to load test Vaadin application with Push communication.