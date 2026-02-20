# 🌉 Bridge Chat Server (Termux)

Simple real-time chat server with bridge mode built using Node.js and Socket.IO.  
Runs on Termux (Android) and supports server-to-server relay.

Install on Termux:

pkg update && pkg upgrade -y  
pkg install nodejs npm -y  
mkdir BridgeChat  
cd BridgeChat  
npm init -y  
npm install express socket.io socket.io-client  

Run Server A:

PORT=3000 node server.js  

Run Server B (Bridge Mode):

PORT=4000 PEER=http://localhost:3000 node server.js  

Open in browser:

http://localhost:3000  
http://localhost:4000  

Project structure:

BridgeChat/  
├── server.js  
├── index.html  
└── package.json  

TRAC Address:  
trac1f7t27ev8katl9rjpnwpx9zl7eygykx77y4dhg2hyqx3nepqtau8qeagz8y  

MIT License
