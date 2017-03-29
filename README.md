webcam-to-server-side-frames
=======

Simple demo app which allows to get frames from webcam through WebRTC and save them on the server side (hard drive) using WebSocket communication.

This app uses part of simple-websocket-server by dpallot: 
https://github.com/dpallot/simple-websocket-server

Usage
-----

1. Clone repo to your /var/www/html dir: 
```
cd /var/www/html
git clone https://github.com/xmementoit/webcam-to-server-side-frames
```
2. On the server side run WebSocket server: 
```
cd webcam-to-server-side-frames
python SimpleWebSocketServer/SimpleExampleServer.py 
```
3. Run your web browser with the following URL:
```
http://localhost/webcam-to-server-side-frames
```
4. You should be asked to permit webcam access allow it.
5. You should see capture your webcam in your browser as well as grabbed frames
   with 1 sec interval. 
6. You should also see series of 'Got frame' messages in the server logs.
7. You can also see series of jpg files containing grabbed frames in your /tmp/ dir:
```
ls /tmp/input*.jpg 
```

Enjoy!!!
---------


