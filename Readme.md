# 🛠️ Whatchat Backend

This repository contains the **backend logic** for Whatchat—a real-time chat application focused on delivering fast, secure, and scalable messaging experiences.

This part of the app handles:
- Database operations
- Socket.IO-based real-time communication
- Core backend logic to improve user experience

---

## 🚀 Upcoming Features

1. **Redis-Based Messaging Queues**
   - Enhance message delivery speed and reliability
   - Enable scalable pub/sub architecture for real-time events

2. **End-to-End Message Encryption**
   - Messages encrypted at the client level
   - Even developers and database admins cannot read user messages
   - Designed with zero-knowledge architecture principles

---

## 🆕 Experimental Features

### Peer-Synced Status Updates (Inspired by WhatsApp Status)
- Users can post ephemeral photo/video/text updates visible to their contacts
- Media is **not stored on the backend**—instead, it’s served directly from the user’s device
- When both users are online, the server coordinates a **silent sync** of status media to the viewer’s device
- Statuses auto-expire after 24 hours and are deleted locally
- Acknowledgement-based syncing ensures privacy and bandwidth efficiency
- Greatly reduces infrastructure cost while improving user control and security

---

## 🔧 Planned Enhancements

### Real-Time Communication
- Socket.IO rooms and namespaces for efficient message routing
- Typing indicators and read receipts
- Offline message queuing and delivery on reconnection

### Security & Privacy
- JWT-based socket authentication during handshake
- Audit logging and anomaly detection
- Rate limiting and abuse protection

### Scalability & Performance
- Redis adapter for horizontal scaling across multiple instances
- Load balancing with sticky sessions (NGINX/Kubernetes)
- Message compression and throttling for large payloads

### Developer Experience
- Modular event handlers for maintainable socket logic
- Live debug dashboard to monitor active sockets and rooms

---

## 📦 Tech Stack

- **Node.js** + **Express.js**
- **Socket.IO** for real-time communication
- **MongoDB** for persistent storage
- **Redis** (planned) for message queuing and caching

---

## 🧠 Vision

Whatchat aims to be a privacy-first, developer-friendly chat platform that scales to thousands of concurrent users. This backend is the foundation for that vision—built with performance, security, and extensibility in mind.

Stay tuned for updates and contributions!
