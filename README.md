# 🚀 Node.js Multi-Stage Dockerfile Example

This repository demonstrates how to build and run a Node.js application using a **multi-stage Dockerfile**. The goal is to create a lean, production-ready Docker image by separating the build and runtime environments.

## 📦 What This Repository Does

* Contains a simple Node.js Express app.
* Uses a **multi-stage Dockerfile** to:

  * Install dependencies and build the app in one stage.
  * Copy only necessary files to a smaller runtime image in the final stage.
* Helps reduce image size and improve performance and security in production.

---

## 🧪 How to Build and Run

### 1️⃣ Clone the Repository

```
git clone https://github.com/AsadR91/nodejs-multistage-Dockerfile.git
cd nodejs-multistage-Dockerfile
```

### 2️⃣ Build the Docker Image

```
docker build -t nodejs-ex -f Dockerfile .
```

This builds the image using the multi-stage Dockerfile, producing a clean and optimized image.

### 3️⃣ Run the Container

```
docker run -d -p 3000:3000 nodejs-ex
```

### 4️⃣ Test It

Visit: [http://localhost:3000](http://localhost:3000)

You should see a simple greeting from the Node.js app.

---

## 🛠️ Why Multi-Stage Builds?

Multi-stage builds allow you to:

* 🚫 Avoid shipping unnecessary build tools in production images.
* 📦 Reduce the final image size significantly.
* 🔐 Improve security and runtime performance.

---

## 📁 Project Structure

```
.
├── Dockerfile              # Multi-stage Dockerfile
├── package.json            # Node.js dependencies
├── index.js                # Simple Express app
└── README.md               # You're reading it!
```

---
<img width="1264" alt="Screenshot 2025-05-19 at 10 13 08 PM" src="https://github.com/user-attachments/assets/74106f7d-4122-42e7-b096-f7f602c7d04e" />

## 📃 License

This project is licensed under the MIT License.

