# 🚀 Real-Time Chat & Social Platform

![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-5.0-092E20?style=for-the-badge&logo=django&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-Upstash-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Neon-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![WebSockets](https://img.shields.io/badge/Protocol-WebSockets-black?style=for-the-badge&logo=socket.io&logoColor=white)
![Deployment](https://img.shields.io/badge/Deployed_on-Render-46E3B7?style=for-the-badge&logo=render&logoColor=white)
![Cloudinary](https://img.shields.io/badge/Cloudinary-3448C5?style=for-the-badge&logo=cloudinary&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Container-2496ED?style=for-the-badge&logo=docker&logoColor=white)

A scalable, full-featured social platform featuring a **high-performance real-time chat system**. Built using **Django Channels** and **ASGI** (Asynchronous Server Gateway Interface) to handle concurrent WebSocket connections, utilizing **Redis** as the message broker for low-latency communication.

## ⚡ Technical Highlights (Why this matters)

This project moves beyond standard HTTP Request-Response cycles by implementing **Event-Driven Architecture**:

* **Asynchronous Python:** Utilizes Python's `async/await` syntax to handle I/O-bound operations (database writes, network calls) without blocking the main thread.
* **WebSockets over HTTP:** Maintains persistent, full-duplex connections for instant bi-directional communication.
* **Redis Pub/Sub:** Acts as the Channel Layer to distribute messages across worker processes efficiently, allowing the application to scale horizontally.
* **Secure & Persistent:** Messages are securely stored in PostgreSQL while media files are offloaded to Cloudinary for optimized delivery.

## 🛠️ Tech Stack

### Backend Infrastructure
* **Core Framework:** Django 5.0 (Python)
* **Real-Time Engine:** Django Channels 4.0
* **Server Interface:** ASGI (Daphne) for handling WebSockets & HTTP
* **Message Broker:** Redis (Upstash)
* **Database:** PostgreSQL (Neon.tech)
* **Authentication:** Django Allauth (Google OAuth2 + Standard Auth)
* **Storage:** Cloudinary API (for profile pics & chat media)

### Frontend & Client
* **JavaScript:** Vanilla JS with native `WebSocket` API (No heavy framework overhead)
* **Styling:** CSS3 (Flexbox/Grid layouts) with Responsive Design
* **Templating:** Django Template Engine (DTL)

### DevOps & Deployment
* **Hosting:** Render (Web Services)
* **CI/CD:** Automated builds via Git hooks
* **Environment Management:** `python-decouple` / Environment Variables

## 📸 Key Features

### 1. Real-Time Messaging System
* **Instant Delivery:** <100ms latency using WebSocket frames.
* **Chat History:** Persistent storage with chronological loading.
* **Media Support:** Send Images and Videos instantly in chat.
* **Message Management:** Delete functionality with real-time DOM updates for all participants.
* **Visual Cues:** Dynamic "Sent/Received" styling and auto-scrolling.

### 2. User & Profile System
* **OAuth Integration:** One-click login with Google.
* **Dynamic Profiles:** Edit bio, profile pictures, and visualize "Visa Journeys" (Custom Data Models).
* **Security:** CSRF protection and Secure (WSS) WebSocket connections.


