
# ⚡ Datagram CLI Node Setup Guide (Linux VPS)

Easily set up your Datagram node on any Linux VPS using this step-by-step guide. Just follow the instructions below and link your license to start earning!

---

## 🧰 Requirements

- Linux VPS (Ubuntu 24.04)
- 2 vCPU, 4GB RAM minimum
- Datagram account: [https://dashboard.datagram.network?ref=611936283]
- Your personal API Key from the dashboard 
![image](https://github.com/user-attachments/assets/bcd084da-a420-46b7-9f07-683d2f862aca)

---

## 🛠️ Setup Instructions

### 1. Update your VPS
```bash
sudo apt-get update && sudo apt-get upgrade -y
sudo apt update && sudo apt install -y wget screen
```

### 2. Download the Datagram CLI
```bash
wget https://github.com/Datagram-Group/datagram-cli-release/releases/latest/download/datagram-cli-x86_64-linux
```

```bash
chmod +x datagram-cli-x86_64-linux
```

```bash
mv datagram-cli-x86_64-linux datagram-cli
```

### 3. Run the node with your API key
```bash
screen -S datagram
```

---

## 🖥️ Run in Background Using `screen`

### Start the node in screen:
```bash
./datagram-cli run -- -key YOUR_API_KEY_HERE
```

### Detach screen (keep running in background):
```bash
Ctrl + A, then press D
```

### Reattach later:
```bash
screen -r datagram
```

---

Wait 30–90 seconds for the device automatically  to appeared

![image](https://github.com/user-attachments/assets/6d069bd4-d3a4-41aa-bc46-d2b5b2fc02ce)

---

## ✅ Done!

You're now running a Datagram node 24/7. Keep it online for maximum rewards!

---

### 💬 Community Help

If you need support, share logs or join the community chat join telegram channel - https://t.me/andhiiTGkamaii

**Made with ❤️ by the community**
