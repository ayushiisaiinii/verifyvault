# 🔐 VerifyVault

### Document Authenticity & Verification System

**"Don’t trust documents. Verify them."**

---

## 🚀 Overview

VerifyVault is a full-stack web application designed to eliminate document fraud by enabling **cryptographic verification of digital documents**.

Institutions can issue tamper-proof documents, and anyone can verify their authenticity instantly — **no login required**.

---

## 🧠 Problem

Document fraud is scaling fast and remains largely unchecked:

* Fake certificates used in jobs and admissions
* No reliable way to verify PDFs shared via WhatsApp or email
* Existing solutions (e.g., DigiLocker, NAD) are not accessible to private institutions
* No mechanism to revoke issued documents

---

## 💡 Solution

VerifyVault replaces blind trust with **verifiable proof** using cryptography.

### Core Capabilities:

* 🔐 **SHA-256 hashing** for tamper detection
* 📱 **QR-based instant verification**
* 👥 **Role-based system** (Issuer, Recipient, Verifier)
* ❌ **Document revocation system**

---

## ⚙️ Tech Stack

### Frontend

* React (Vite)
* React Router
* Axios

### Backend

* Node.js
* Express.js
* JWT Authentication
* Multer (file uploads)
* Crypto (SHA-256 hashing)
* QR Code generation

### Database & Storage

* MongoDB Atlas
* Cloudinary (documents + QR storage)

### Deployment

* Vercel (Frontend)
* Render (Backend)

---

## 🔁 System Workflow

### 📤 Document Issuance Flow

1. Issuer logs in
2. Uploads document
3. File is stored on Cloudinary
4. SHA-256 hash is generated
5. Unique verification code is created
6. QR code is generated
7. Metadata stored in MongoDB

---

### 🔍 Verification Flow

Users can verify documents via QR code or verification code:

* ❌ **Not Found** → Document is fake
* 🚫 **Revoked** → Issuer has invalidated it
* ⚠️ **Tampered** → Hash mismatch detected
* ✅ **Genuine** → Document is authentic

---

## 📊 Features

* ✔️ Tamper-proof document validation
* ✔️ QR-based verification (no authentication required)
* ✔️ Role-based dashboards
* ✔️ Document revocation capability
* ✔️ Secure cloud storage
* ✔️ Fully deployed and production-ready

---

## 🧪 Performance

* ⚡ Verification time: **< 2 seconds**
* 📤 Upload time: **< 5 seconds** (≤ 5MB files)
* 🧾 Supported formats: **PDF, Images**

---

## 🔮 Future Scope

* 📱 Mobile app with built-in QR scanner
* ⛓️ Blockchain integration (Ethereum / Polygon)
* 🏛️ Integration with DigiLocker & NAD
* 📊 Verification analytics dashboard
* 📦 Bulk document issuance
* 🔏 Digital signatures (X.509 standard)

---

## 📌 Key Highlight

VerifyVault is not just a prototype — it is a **live, working system** solving a real-world problem with practical cryptographic implementation.

---

## ⭐ Final Thought

Anyone can generate a PDF.
**VerifyVault proves whether it’s real.**
