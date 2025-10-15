# Super Clipboard

Super Clipboard is a lightweight self-hosted clipboard and text/file relay service designed for restricted environments such as NAT, VNC, or cloud consoles.  
It allows you to securely transfer text and files between devices or servers without relying on public IPs or SSH access.

---

## 🚀 Features

- **Clipboard relay:** Quickly push and pull text between devices.
- **File sharing:** Supports file uploads and direct-link sharing.
- **Auto cleanup:** Optional expiration and self-destruction.
- **Standalone deployment:** Backend and frontend served together on port `5173`.
- **Persistent data:** All data is stored under `/app/backend/storage`.

---

## 🧩 Deployment

This ClawCloud Run template deploys a single instance using a `StatefulSet` and exposes the web interface via port `5173`.

**Default configuration**
- Port: `5173`
- Timezone: `Asia/Shanghai`
- Persistent path: `/app/backend/storage`

