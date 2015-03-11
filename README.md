# json-live
Live json data structures maintained across server client via Socket.io

This should solve the irritating problem of having to manually send commands to update json files across server and clients.

##API

Create a live json object 
```js
var json = new JSONLive(socket);
//socket is an active socket.io object
```

Add a new JSON object
```js
json.create("Myjson");
```

Patch
```js
json.patch("...");
//this will be the standard protocol for patching json
//maybe using json-patch
```
