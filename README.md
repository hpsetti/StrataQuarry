# ⛏️ Strata Quarry

> **Build cloud infrastructure from first principles.**
>
> Strata Quarry is a **self-hosted object storage service** inspired by cloud storage solutions, but lightweight and easy to run on your own infrastructure.  
It is built with **Node.js + Nitro** and designed for developers who want full control over their data without depending on third-party providers.


## ✨ Why?

- You want a **private alternative** to S3 for small projects or local dev
- You’re learning how object storage systems are built under the hood
- You want to run your own storage service on **local hardware** or **cloud VMs**

## 🚀 Features

### ✅ Current

* 🪣 Bucket creation
* 💾 Filesystem storage
* 📄 Zod validation
* ⚡ Nitro API routes
* 🛡️ Structured error handling
* 🔷 TypeScript

### 🛣️ Coming Soon

* 📁 Object upload & download
* 🔍 Object listing
* 🔐 Authentication & IAM
* 🔗 Signed URLs
* 📦 Multipart uploads
* 🌍 Distributed storage
* 📊 Metrics & monitoring
* 💻 CLI & SDK

---

## 🏗️ Architecture

```text
Client
   │
   ▼
Nitro Routes
   │
   ▼
Services
   │
   ▼
Storage
   │
   ▼
Filesystem
```

Each layer has one responsibility, keeping the code simple and easy to understand.

---

## 📂 Project Structure

```
deccan-vault/
├── server/
│   ├── middleware/          # Global middleware (e.g., error handling, logging)
│   ├── routes/              # REST API endpoints
│   └── utils/               # Utilities (custom errors, helpers)
├── .gitignore
├── package.json
└── README.md
```

---

## 🚀 Installation

### Prerequisites

* Node.js 20+
* pnpm (recommended)

### Installation

```bash
git clone https://github.com/<your-username>/strata-quarry.git

cd strata-quarry

pnpm install
```

### Run the development server

```bash
pnpm dev
```

The API will be available at:

```text
http://localhost:3000
```

## 🧪 Quick Test

```bash
curl http://localhost:3000/health
```

Expected response

```json
{ "status": "ok", "service": "DeccanVault" }
```


---

## 🗺️ Roadmap

* ✅ Foundation
* ✅ Bucket Management
* 🚧 Bucket API
* ⏳ Object Storage
* ⏳ Security & IAM
* ⏳ Signed URLs
* ⏳ Production Features
* ⏳ Distributed Storage
* ⏳ Enterprise Features


---

## 📜 License

MIT License - free to use, modify, and self-host.
