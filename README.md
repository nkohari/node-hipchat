A simple node.js library for communicating with the [HipChat](http://hipchat.com/) REST API.
Still under construction, and currently only supports sending messages to rooms.

You can also install via npm:

	npm install node-hipchat

# Examples

First make sure you have an [Admin API Key](https://www.hipchat.com/admin/api).

## Send a message to a room

    var hipchat = require('node-hipchat');

    var HC = new hipchat('YOUR_API_KEY');

    HC.listRooms(function(data) {
      console.log(data); // These are all the rooms
    });

    var params = {
      room: 123456, // Found in the JSON response from the call above
      from: 'FunkyMonkey',
      message: 'Some HTML <strong>formatted</strong> string',
      color: 'yellow'
    };

    HC.postMessage(params, function(data) {
      // Message has been sent!
    });
