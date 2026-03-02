🚀 PeerSetup

A lightweight, event-driven WebRTC helper that simplifies browser-to-browser video connections.
PeerSetup abstracts the complexity of:
📷 Camera & microphone initialization
🔄 Offer / Answer negotiation
❄️ ICE candidate buffering
🎬 Local & remote media track handling
🧹 Graceful connection cleanup

📖 Documentation Preview
<p align="center"> <a href="./lib.png"> <img src="../lib.png" alt="PeerSetup Documentation Preview" width="850"/> </a> </p>
✨ Features

# Simple API
Built on native WebRTC
Custom event system (on, off, emit)
Lightweight & framework agnostic
MIT Licensed

🛠 Installation 
npm i nahdi-flowrtc and then 
Just import the class:
import { PeerSetup } from "./PeerSetup.js";

🎯 Basic Usage
<pre>
  <code>
    const peer = new PeerSetup({
  localVideoRef: document.getElementById("localVideo"),
  remoteVideoRef: document.getElementById("remoteVideo"),
  constraint: { video: true, audio: true }
});

peer.on("candidate", (candidate) => {
  // send candidate to signaling server
})
  </code>
</pre>


🤝 Contributing

Contributions, suggestions, and improvements are welcome.

If you like the project, consider giving it a ⭐ on GitHub.
