Based on `nkohari/node-hipchat`
A simple node.js library for communicating with the [HipChat](http://hipchat.com/) REST API.
Still under construction, and currently only supports sending messages to rooms.

You can also install via npm:

  npm install node-hipchat


Methods implemented:
====================

rooms/create   createRoom (params, callback)  
rooms/delete:  deleteRoom(room, callback)  
rooms/history: getHistory(room, callback)  
rooms/list:     listRooms(callback)  
rooms/message: postMessage(params, callback)  
rooms/show:     showRoom(room, callback)  

users/create   createUser(params, callback)  
users/delete   deleteUser(user_id, callback)  
users/list     listUsers(callback)  
users/show     showUser(user_id, callback)  
users/update   updateUser(params, callback)  


