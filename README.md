# DSy-webrtc

A simple WebRTC implementation using WebSockets for signaling.

## Project Overview

This project demonstrates a basic WebRTC peer-to-peer connection using a WebSocket server for signaling (SDP exchange and ICE candidates).

- **`server.js`**: A Node.js server using `express` and `ws` to handle static file serving and WebSocket broadcasting for signaling.
- **`index.html`**: The client-side application that uses the WebRTC API to establish a data channel connection between peers.
- **`package.json`**: Contains project dependencies (`express`, `ws`).

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) installed on your machine.

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd example-webrtc
   ```

2. Install the dependencies:
   ```bash
   npm install
   ```

### Running the Application

1. Start the server:
   ```bash
   node server.js
   ```

2. Open your web browser and navigate to `http://localhost:4000`.

3. To test the peer-to-peer connection, open the same URL in a second browser window or an incognito tab.

4. Click the **Connect** button in both windows to initiate the signaling process.
5. Once connected, you can type a message in one window and click **Send** to see it appear in the other window.

## Technologies Used

- **WebRTC**: For peer-to-peer data communication.
- **WebSockets (`ws`)**: For the signaling server.
- **Express**: For serving the static HTML file.
- **JavaScript**: For both client-side and server-side logic.
