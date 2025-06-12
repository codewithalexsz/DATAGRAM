# DATAGRAM

# 📡 Datagram CLI Setup Guide

This guide will walk you through registering on the Datagram network, setting up the CLI tool, and running it inside a `screen` session for stability and background execution.

---

## 📝 Step 1: Register on Datagram Network

1. Visit the Dashboard:  
   👉 [https://dashboard.datagram.network?ref=602038144](https://dashboard.datagram.network?ref=602038144)

2. Register using your **email address**.

3. Once registered, **copy your API key** from the **Wallet Licenses** section.

---

## 📁 Step 2: Create Datagram Directory and download cli file

Create a working directory to organize your Datagram files:

```bash
mkdir datagram
cd datagram
```
```bash
wget https://github.com/Datagram-Group/datagram-cli-release/releases/latest/download/datagram-cli-x86_64-linux
chmod +x datagram-cli-x86_64-linux
```

## 🖥️ Step 4: Run Datagram in a screen Session
Using screen ensures that Datagram keeps running even if your terminal disconnects.

Start a screen session:

```bash
screen -S datagram
```

# 5:  Run the CLI with your API key (replace YOUR_API_KEY with the one from your Wallet Licenses):

```bash
./datagram-cli-x86_64-linux run -- -key YOUR_API_KEY
```

# Detach from the screen session safely by pressing:
```bash
CTRL + A then D
```

# Reattach to Datagram Screen To view the running process again:
```bash
screen -r datagram
```

# If the screen is already attached elsewhere, reattach with:
```bash
screen -d -r datagram
```

Ensure your machine is kept running or managed via tmux/screen/systemd for uptime.
