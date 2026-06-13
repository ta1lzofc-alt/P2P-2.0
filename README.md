# 🔗 P2P Chat

Peer-to-peer messaging application using WebRTC technology with Python signalling server.

## ✨ Features
- Direct P2P connection via WebRTC Data Channel
- No message routing through server after connection
- Automatic peer discovery via WebSocket signalling
- Real-time messaging with low latency
- Works in local network without internet access
- Simple Python server and browser-based client

## 🛠 Tech Stack
- **Backend**: Python, WebSockets (asyncio/websockets)
- **Frontend**: HTML5, CSS3, JavaScript
- **P2P**: WebRTC (RTCPeerConnection, Data Channel)

## 📡 How it works
1. Clients connect to WebSocket signalling server
2. Server assigns unique peer IDs
3. Peers exchange SDP offers/answers and ICE candidates
4. Direct WebRTC Data Channel established
5. Messages flow directly between browsers

## 🚀 Quick Start
```bash
# Install dependencies
pip install websockets

# Run signalling server
python server.py

# Open client.html in two browsers
# Enter peer IDs and start chatting!
