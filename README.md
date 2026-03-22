# 🚀 ZoomatoCode – Microservices Food Delivery Platform

A scalable, Zomato-like food delivery application built using **microservices architecture**, featuring real-time order tracking, event-driven communication, and secure online payments.

---

## 📌 Overview

TomatoCode is a full-stack food delivery platform designed to simulate real-world systems. It follows a **loosely coupled microservices architecture**, where each service handles a specific domain and communicates asynchronously using a message broker.

---

## 🧩 Architecture

- Microservices-based system  
- Event-driven communication using **RabbitMQ**  
- Real-time updates using **Socket.io**  
- Independent services for scalability and maintainability  

---

## ⚙️ Services

### 🔐 Auth Service
- User authentication and authorization  
- JWT-based login/signup  

### 🧰 Utils Service
- File uploads (images, documents)  
- Payment integration (Razorpay & Stripe)  

### 🍽️ Restaurant Service
- Add/update restaurants  
- Manage menu, availability (open/close)  
- Handle orders, cart, and addresses  

### 🚴 Rider Service
- Rider profile management  
- Accept and manage delivery orders  

### 📡 Realtime Service
- Real-time communication using Socket.io  
- Live order tracking and status updates  

### 🛠️ Admin Service
- Approve/reject restaurants and riders  
- Platform-level management controls  

---

## 🔁 System Flow (High-Level)

1. User places an order  
2. Restaurant Service processes the order  
3. Event is published to RabbitMQ  
4. Rider Service consumes the event and assigns delivery  
5. Realtime Service pushes live updates via Socket.io  

---

## 🛠️ Tech Stack

**Frontend:**  
- React.js  

**Backend:**  
- Node.js  
- Express.js  

**Database:**  
- MongoDB  

**Communication & Realtime:**  
- RabbitMQ (Message Broker)  
- Socket.io  

**Payments:**  
- Razorpay  
- Stripe  

---

## 🔐 Key Features

- Microservices-based scalable architecture  
- Event-driven communication (RabbitMQ)  
- Real-time order tracking (Socket.io)  
- Secure payment integration  
- Admin approval workflows  
- Modular and maintainable backend design  

---

## 📷 Architecture Diagram

> Upload your diagram inside repo (e.g. `/docs/architecture.png`) and update below path

![Architecture Diagram](./docs/architecture.png)

---

## 🚀 Getting Started

### Prerequisites
- Node.js  
- MongoDB  
- RabbitMQ  

---

## 📌 Future Improvements

- API Gateway implementation  
- Rate limiting & caching (Redis)  
- CI/CD pipeline  

---

## 🏷️ Badges

![Node.js](https://img.shields.io/badge/Node.js-Backend-green)
![Microservices](https://img.shields.io/badge/Architecture-Microservices-blue)
