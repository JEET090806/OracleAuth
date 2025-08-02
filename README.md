# 🛡️ **OracleAuth**

**OracleAuth** is a **decentralized, real-time identity verification system** built for privacy, speed, and security. It allows users to generate secure QR codes from personal data (Name, UID, DOB, Email), hashed using **SHA-256** and stored securely in **Firebase**.

These QR codes can then be scanned by **authorized personnel** to instantly retrieve and verify the associated identity — without ever exposing raw data.

> 🔗 **Live Demo**: [oracleauth-98c39.web.app](https://oracleauth-98c39.web.app)

---

## 🧠 **How It Works**

```text
┌──────────────┐    ┌────────────────┐    ┌───────────────┐
│ User Input   │ ─▶│ SHA-256 Hash   │ ─▶ │ QR Code Gen   │
└──────────────┘    └────────────────┘    └───────────────┘
                                                  │
┌──────────────┐    ┌────────────────┐    ┌───────────────┐
│ Verification │ ◀─│ QR Extraction  │ ◀─ │ QR Scanner    │
└──────────────┘    └────────────────┘    └───────────────┘
```

✅ The QR code contains **only the hashed data** — not the original information.  
🔒 The hash is looked up in the **Firebase Realtime Database** to verify the identity.  
🚫 If an unauthorized user scans the QR, they will see **only the hash**, which is not reversible.

---

## 🔧 **Tech Stack**

| **Component**        | **Technology**                             |
|----------------------|---------------------------------------------|
| 🖥️ Frontend           | HTML, CSS, JavaScript                      |
| 🔐 QR Generation      | `qrcode.min.js`                            |
| 📷 QR Scanning        | `html5-qrcode` (webcam-based scanning)     |
| 🧮 Hashing Algorithm  | `crypto-js` (SHA-256)                      |
| 🗃️ Database           | Firebase Realtime Database                 |
| ☁️ Hosting            | Firebase Hosting                          |

---

## ✨ **Features**

- 🔐 **SHA-256 encryption** of all sensitive identity data  
- 📷 **Webcam-based QR scanning** for real-time identity lookup  
- ⚡ **Instant verification** using Firebase’s fast, cloud-based backend  
- 🧾 **No personal data stored in the QR code** — only the hash  
- 🌐 **Firebase-powered** architecture for speed, scale, and security  

---

## 🔐 **Security & Privacy**

✔️ **One-way encryption** — hashes are irreversible  
✔️ **QR codes contain only hashes**, no raw PII  
✔️ **Only trusted systems** can access user data via Firebase  
✔️ **No centralized identity leak risk** — everything is isolated, hashed, and controlled

---

## 📚 **Documentation**

You’ll find all documentation within the interface under the **Docs** section. Key areas include:

- ✅ **Getting Started** – How to use the QR generator & scanner  
- 🔌 **API Reference** – Firebase structure and access logic  
- 🔐 **Security Best Practices** – Guidance for safe implementation  
- ⚙️ **Advanced Features** – For developers and enterprise use  

👉 Explore it at: [oracleauth-98c39.web.app/#docs](https://oracleauth-98c39.web.app/#docs)

---

## 🚀 **Future Enhancements**

- 🔗 **Blockchain integration** for tamper-proof logs  
- 📱 **Mobile app** (Android/iOS) for on-the-go scanning  
- 🧠 **Fraud alerts** via duplicate detection and pattern matching  
- 🧩 **Role-based access control** for admin, verifier, etc.

---

## 📄 **License**

Licensed under the **MIT License** — free to use, share, and modify.

---

## 🙋 **Support & Contributions**

Have an idea, bug, or question?

- 📂 Contact :
    jeetpandya2006@gmail.com
    tanikshashah2409@gmail.com

---
