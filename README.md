# Rocketgraph Installer

The official Windows installer for [Rocketgraph](https://rocketgraph.com).

Looking for alternative install methods? Check out [other install options here](https://github.com/Rocketgraphai/install).

## Download

📦 [Download the latest version](https://github.com/rocketgraphai/rocketgraph-setup/releases/latest)

## Requirements
- Windows 10 or later
- Virtualization enabled in BIOS/UEFI
- Internet connection (for updates)

##  Installation

1. Download the `.exe` file from [Releases](https://github.com/rocketgraphai/rocketgraph-setup/releases).
2. Run the installer.
3. Follow the prompts to complete setup. [(See the installer guide)](docs/v1.3/welcome.md)

## What This Installer Does

- Installs the **latest version of Rocketgraph** automatically using Docker
- Sets up the required **Docker Compose configuration**
- Installs **Docker Desktop** (if not already installed)
- Enables necessary Windows features:
  - **Windows Subsystem for Linux (WSL 2)**
  - **Virtual Machine Platform**

## Troubleshooting

### ⚠️ Antivirus Warning

Some antivirus programs may flag the installer because it is not yet code-signed. This is a common false positive for unsigned software. Rest assured, the installer is safe and has not been tampered with.

---

### 🔄 Reboot Required for WSL 2 or VM Platform

If your system does not have **WSL 2** or the **Virtual Machine Platform** enabled, the installer will attempt to enable them for you. This process may require a **system reboot**.

> After the reboot, please **rerun the installer manually** to complete the installation.

To avoid this, ensure the following Windows features are already enabled:
- **Windows Subsystem for Linux**
- **Virtual Machine Platform**

You can enable these manually via Windows Features or PowerShell before running the installer.
