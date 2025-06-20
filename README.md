🛡️ OracleAuth
OracleAuth is a decentralized, real-time identity verification system built for privacy and speed. It enables users to generate secure QR codes from their personal data (name, UID, DOB, email), which are hashed using SHA-256 and stored in Firebase. These QR codes can then be scanned by authorized personnel to retrieve and verify user data — securely and instantly.

🔗 Live Demo: oracleauth-98c39.web.app

🧠 How It Works
css
Copy
Edit
┌──────────────┐    ┌────────────────┐    ┌───────────────┐
│ User Input   │ ─▶│ SHA-256 Hash   │ ─▶ │ QR Code Gen   │
└──────────────┘    └────────────────┘    └───────────────┘
                                                  │
┌──────────────┐    ┌────────────────┐    ┌───────────────┐
│ Verification │ ◀─│ QR Extraction  │ ◀─ │ QR Scanner    │
└──────────────┘    └────────────────┘    └───────────────┘
The QR code contains only the hash — not personal data — and only your internal Firebase database can resolve that hash back to user info.

🔧 Tech Stack
Component	Tech Used
Frontend	HTML, CSS, JavaScript
QR Generation	qrcode.min.js
QR Scanning	html5-qrcode (webcam-based scanning)
Hashing Algorithm	crypto-js (SHA-256)
Realtime Database	Firebase Realtime Database
Hosting	Firebase Hosting

✨ Features
🔐 SHA-256 encryption of sensitive data before QR generation

📷 QR scanning via device webcam with live data retrieval

⚡ Instant lookup from Firebase using hashed key

🛡️ Hash-only QR content: no personal data embedded in the QR

🌐 Firebase-based hosting & database for fast and secure access

🔐 Security & Privacy
All user data is hashed before storage.

QR codes expose nothing except the SHA-256 hash.

Only authorized systems connected to Firebase can query records.

Hashes are non-reversible, even if intercepted.

📚 Documentation
OracleAuth's documentation is built into the interface. Key areas include:

✅ Getting Started — Using the QR generator and scanner

🔌 API Reference — Firebase structure and hash key logic

🔐 Security Best Practices — Keeping identities safe

⚙️ Advanced Features — Extend OracleAuth for broader use cases

You can explore the documentation directly on the OracleAuth Website.

📌 Future Enhancements
🔗 Blockchain integration for tamper-proof verification logs

📱 Native mobile app support for scanning and verifying on the go

🧠 Smart alerts for fraudulent or duplicate entries

🧩 Role-based access for scan permissions

📄 License
This project is licensed under the MIT License.

🙋 Support
For issues, improvements, or contributions, visit the repo:
👉 github.com/JEET090806/OracleAuth
 
