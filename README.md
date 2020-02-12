# django_websocket_demo

A very basic Django 3.0 application that uses WebSockets.

Install the requirements.
Start the server with: 

`$ uvicorn websocket_app.asgi:application`

Go to your browser's Console and type the following:

`ws = new WebSocket('ws://localhost:8000/')`

`ws.onmessage = event => console.log(event.data)`

`ws.send("ping")`

And you shall receive "pong!" from the ASGI server.
