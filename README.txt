Wartanks Online Render Fixed

IMPORTANT:
Do not delete the public folder files. Render runs server.js, and server.js serves the browser game from public/.

Render settings:
Build Command: npm install
Start Command: npm start

Open the Render app URL in the browser, for example:
https://your-app-name.onrender.com

Do not open index.html locally when testing the Render server, unless you pass a server URL:
index.html?server=wss://your-app-name.onrender.com

Health check:
https://your-app-name.onrender.com/health

This fixed build includes:
- public/ static files
- emergency root fallback for index.html/styles.css/game.js
- WebSocket heartbeat
- clearer disconnect message
- same gameplay as online alpha
