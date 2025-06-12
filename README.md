
# ⚡ Datagram CLI Node Setup Guide (Linux VPS)

Easily set up your Datagram node on any Linux VPS using this step-by-step guide. Just follow the instructions below and link your license to start earning!

---

Then run:
```bash
chmod +x datagram-cli-x86_64-linux
mv datagram-cli-x86_64-linux datagram-cli
```

---

## 🧰 Requirements

- Linux VPS (Ubuntu 20.04 or 22.04)
- 2 vCPU, 4GB RAM minimum
- Datagram account: [https://dashboard.datagram.network?ref=611936283]
- Your personal API Key from the dashboard![image](https://github.com/user-attachments/assets/8519d0ef-707d-4d1f-9ba6-d74c2f10bcbd)


---

## 🛠️ Setup Instructions

### 1. Update your VPS
```bash
sudo apt update && sudo apt install -y wget screen
```

### 2. Download the Datagram CLI
```bash
wget https://github.com/Datagram-Group/datagram-cli-release/releases/latest/download/datagram-cli-x86_64-linux
chmod +x datagram-cli-x86_64-linux
mv datagram-cli-x86_64-linux datagram-cli
```

### 3. Run the node with your API key
```bash
./datagram-cli run -- -key YOUR_API_KEY_HERE
```

---

## 🖥️ Run in Background Using `screen`

### Start the node in screen:
```bash
screen -S datagram
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

## 🔗 Link Your Node to Dashboard

1. Visit: [https://dashboard.datagram.network](https://dashboard.datagram.network)
2. Wait 30–90 seconds for the device to appear
3. Select the device
4. Click **"Link License"**

---

## 🔁 Auto-start on VPS Reboot (Optional)

Run:
```bash
crontab -e
```

Then add:
```bash
@reboot screen -dmS datagram /root/datagram-cli run -- -key YOUR_API_KEY_HERE
```

Replace `/root/` with the correct path to your binary.

---

## ✅ Done!

You're now running a Datagram node 24/7. Keep it online for maximum rewards!

---

### 💬 Community Help

If you need support, share logs or join the community chat.

**Made with ❤️ by the community**
