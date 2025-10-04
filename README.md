# Bluetooth Auto DoS Script

> ⚠️ **IMPORTANT — Use only for authorized testing and security research.**  
> Do **not** run this against devices or networks you do not own or do not have explicit permission to test. Misuse may be illegal and unethical.

A lightweight Python script to automate Bluetooth denial-of-service testing on Kali Linux. This repository provides a simple, easy-to-run tool intended for educational and authorized penetration testing scenarios.

---

## Features

- Simple, single-file Python attack script  
- Designed for Kali Linux environments  
- Minimal setup — clone and run  
- Clear pre-run checks to ensure your Bluetooth adapter is ready

---

## Requirements

- Kali Linux (recommended)
- Python (as required by `attack.py`)
- Bluetooth adapter supported by `hciconfig`

---

## Installation (Kali Linux)

```bash
git clone https://github.com/07iamravi/Bluetooth-autodos
cd Bluetooth-autodos
```

---

Before you run

Make sure your Bluetooth adapter is up and in the correct mode. Use hciconfig to inspect the adapter.

1. Check adapter status
```bash
hciconfig
```

Look for your Bluetooth interface (e.g., hci0) and confirm it is UP. If the interface is down, bring it up:

2. Bring adapter up (if needed)
```bash
sudo hciconfig hci0 up
```
> Note: Some attacks or tools require the adapter to be in monitor/management mode supported by your chipset and drivers. Confirm your adapter supports the needed features before proceeding.




---

Running

Once pre-checks are complete and you have legal authorization, run the script:
```bash
sudo python attack.py
```

(Use python3 if your system maps Python 3 to python3.)


---

Safety & Legal

This project is provided for educational purposes only. You are responsible for ensuring your actions comply with local laws and organizational policies. Never target devices or networks without explicit permission.
