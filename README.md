# S3mail
S3mail — A Cloud-Native IMAP Server for Object Storage

S3mail is a lightweight, stateless IMAP server that stores and serves full email mailboxes directly from S3-compatible object storage. Designed to replace traditional mail storage (like Maildir/mbox) with modern, scalable, cloud-friendly infrastructure.


## 🚀 Features

- 💾 Store entire mailboxes in S3 (or MinIO, Wasabi, etc.)
- 📬 IMAPv4 protocol support (RFC 3501)
- 🔐 Pluggable authentication (local, OIDC, LDAP)
- 🌐 Stateless design — perfect for containers and Kubernetes
- 📂 MIME-compliant message storage (RFC 5322)
- ⚙️ Written in **Rust** for safety & performance (or Go — TBD)

## 🔧 Use Cases

- Cloud-native mail hosting
- Lightweight self-hosted inboxes
- Serverless mail ingestion pipelines
- Cost-effective mail storage at scale

## 🛠️ Tech Stack

- Rust (or Go) + async runtime (Tokio or goroutines)
- Native S3 SDK (AWS S3, MinIO, Wasabi, etc.)
- IMAP server engine
- TLS/STARTTLS support

## 📦 Installation (WIP)

```bash
docker run -p 143:143 s3mail/s3mail

## 🛣️ Roadmap

- [x] Store/retrieve RFC 5322 messages in S3
- [ ] Read-only IMAP (LIST, FETCH)
- [ ] Write support (APPEND, STORE, DELETE)
- [ ] Multi-user support
- [ ] TLS, authentication (PAM, OIDC)
- [ ] Web admin UI (optional)

---

## 🤝 Contributing

We welcome early contributors! Help us:

- 🧩 Build protocol handlers
- 🧪 Test with real mail clients (Thunderbird, Apple Mail, etc.)
- 💾 Improve storage backends (S3, MinIO, etc.)
- 🧭 Shape the roadmap

---

## 📄 License

This project is open-source under the  **Apache-2.0** license .
