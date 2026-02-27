# nscan

<p align="center">
  <img src="https://raw.githubusercontent.com/sandipduley/upload-images/main/Nscan.png"
       alt="Dockerised Neovim Preview"
</p>

nscan is a fast, asynchronous Nmap wrapper with a live Rich-powered terminal UI that displays real-time port scanning results in a clean, structured format

---

## Features

- Real-time scan progress
- Clean Rich terminal UI
- Open port tracking
- Lightweight & fast
- Standalone Linux executable

---

## Requirements

- Linux
- nmap installed

---

### Debian-based disto

```bash
sudo apt update
sudo apt install nmap git
git clone --depth=1 https://github.com/sandipduley/nscan.git
cd nscan
```

### Arch-based distro

```bash
sudo pacman -Sy nmap git
git clone --depth=1 https://github.com/sandipduley/nscan.git
cd nscan
```

## Make executable and install system-wide

```bash
chmod +x nscan
sudo cp nscan /usr/local/bin/nscan
```

## Verify installation

```bash
nscan --help
```

## Usage

#### Basic scan

```bash
nscan example.com -v
```

#### Scan all ports

```bash
nscan example.com -p- -v
```

#### Aggressive timing

```bash
nscan example.com -T4
```

## Disclaimer

## This tool is intended for authorized security testing and educational purposes only. Do not scan systems without permission.
