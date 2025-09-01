# XMRig VRL ARM Build for Virel

This repository contains a precompiled **XMRig VRL binary for ARM devices** (Android/Ubuntu/Termux) optimized for mining **Virel (VRL)**.  

> ⚠️ This build is specifically for ARM64 CPUs and may not work on x86/x64 devices.

---

## Features

- Optimized for **ARM Cortex-A series** (Android, Termux, Ubuntu ARM VMs)
- Ready to mine **Virel (VRL)** using **RandomX/VRL** algorithm
- Supports TLS/SSL pool connections
- Minimal setup: no compilation required
- Configurable threads for best performance on low-memory ARM devices

---

## Requirements

- **ARM64 CPU**
- **Linux-based OS** (Android via Termux, Ubuntu ARM, Debian ARM)
- **~2-4 GB free RAM** for RandomX dataset
- **Internet connection** for pool mining

> Huge Pages are **not supported** on most Android/VM kernels. The miner will run using normal memory.

---
## Ubuntu
```
pkg update -y && pkg upgrade -y
pkg install proot-distro -y
```
### Install Ubuntu (for example  22.04)
```
proot-distro install ubuntu-22.04
```
### Jalankan Ubuntu
```
proot-distro login ubuntu-22.04
```
### download
```
git clone https://github.com/nheoshikuyanhemo/xmrig-virel-arm-build.git
```

## Usage

1. Make the binary executable:
```
chmod +x xmrig
```

### Run the miner:

```
./xmrig -a randomvirel --url <POOL_ADDRESS:PORT> --tls --user <YOUR_WALLET_ADDRESS.WORKER_NAME>
```

### example

```
./xmrig -a randomvirel --url asia.rplant.xyz:17155 --tls --user v16jfoyeh9q6iuzzlim6umncx7ljgbc6ep8sngi.Eixa
```


## If you find this build helpful, you can donate Virel (VRL) to support development:
```
v16jfoyeh9q6iuzzlim6umncx7ljgbc6ep8sngi
```

### License

The miner is XMRig VRL, follow its official license

Precompiled ARM binary provided as-is, use at your own risk
