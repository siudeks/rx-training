
# Step 3

Create REST / Websocket endpoints to allow remotely watching folder(s) defined on server-side
Use rest to initiate connection - initially you need to as about current folder structure
Use Websocket to send data to client (data means current folder structure and future changes in folder structure)
Define simple rest endpoint to allow remotely create folder / files for testing purposes
Include full integration tests
<br /><br />

**Tips**<br />
Websocket - if you are not able connect localhost socket, check socket configuration:

```registry.addEndpoint("/websocket").setAllowedOrigins("*").withSockJS();```
