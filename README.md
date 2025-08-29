# FANSPEED-CONTROL-DELL-TUI

![Platform](https://img.shields.io/badge/Platform-Linux-blue.svg)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![GitHub issues](https://img.shields.io/github/issues/LINUX-OASIS/FANSPEED-CONTROL-DELL-TUI)](https://github.com/LINUX-OASIS/FANSPEED-CONTROL-DELL-TUI/issues)
[![GitHub pull requests](https://img.shields.io/github/issues-pr/LINUX-OASIS/FANSPEED-CONTROL-DELL-TUI)](https://github.com/LINUX-OASIS/FANSPEED-CONTROL-DELL-TUI/pulls)
[![GitHub stars](https://img.shields.io/github/stars/LINUX-OASIS/FANSPEED-CONTROL-DELL-TUI?style=social)](https://github.com/LINUX-OASIS/FANSPEED-CONTROL-DELL-TUI/stargazers)
![Bash script](https://img.shields.io/badge/Language-Bash_script-black?logo=gnubash)

A simple yet powerful Bash script with a Terminal User Interface (TUI) to manage fan speeds on Dell laptops. Take control of your system's thermals with pre-defined profiles for stock, low, and maximum fan speeds.

---

## ✨ Features

*   **💻 TUI-based Menu**: An easy-to-use `whiptail` interface for straightforward operation.
*   **⚙️ Multiple Fan Profiles**: Instantly switch between **[STOCK]**, **[LOW]**, and **[MAX]** fan profiles.
*   **🌡️ Persistent Max Speed**: The **[MAX]** profile creates a `systemd` service to keep fans at full blast for demanding tasks, surviving reboots and system overrides.
*   **📊 Status Check**: Quickly view the currently active fan profile.
*   **🚀 Automatic Dependency Handling**: The script automatically checks for the required `i8kutils` dependency and prompts to install it if missing.

## 🐧 OS Compatibility

This script is designed for Debian-based Linux distributions that use the `apt` package manager. It has been tested and is known to be compatible with:

*   ✅ Debian
*   ✅ Ubuntu
*   ✅ Linux Mint
*   ✅ Other Debian/Ubuntu derivatives (e.g., Pop!_OS, Zorin OS)

> **Hardware Note**: This utility relies on the `dell-smm-hwmon` kernel module, and is therefore only compatible with Dell laptops that support this module.

## 🛠️ Dependencies

The script requires the following packages:

*   `i8kutils`: The core utility for interfacing with Dell's SMM BIOS for fan control.
*   `whiptail`: A utility for creating dialog boxes from shell scripts (typically pre-installed).

The script will automatically check for `i8kutils` and will offer to install it for you if it's missing.

## 🚀 Usage

1.  Clone the repository:
    ```bash
    git clone https://github.com/LINUX-OASIS/FANSPEED-CONTROL-DELL-TUI.git
    cd FANSPEED-CONTROL-DELL-TUI
    ```

2.  Make the script executable:
    ```bash
    chmod +x custom-FANSPEED-CONTROL-DELL.sh
    ```

3.  Run the script with `sudo` privileges:
    ```bash
    sudo ./custom-FANSPEED-CONTROL-DELL.sh
    ```
    > **Note:** `sudo` is required because the script modifies system configuration files (`/etc/i8kmon.conf`) and manages `systemd` services.

## 💬 Contributing

[Pull requests](https://github.com/LINUX-OASIS/FANSPEED-CONTROL-DELL-TUI/pulls), [issues](https://github.com/LINUX-OASIS/FANSPEED-CONTROL-DELL-TUI/issues), and suggestions are warmly welcomed!
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## 🌐 Links

*   [Issues](https://github.com/LINUX-OASIS/FANSPEED-CONTROL-DELL-TUI/issues)
*   [Pull Requests](https://github.com/LINUX-OASIS/FANSPEED-CONTROL-DELL-TUI/pulls)
*   [Releases](https://github.com/LINUX-OASIS/FANSPEED-CONTROL-DELL-TUI/releases)
*   [Wiki](https://github.com/LINUX-OASIS/FANSPEED-CONTROL-DELL-TUI/wiki)

## 🧙‍♂️ Maintainer

*   [**LINUX-OASIS**](https://github.com/LINUX-OASIS)

## 📜 License

This project is licensed under the **GNU General Public License v3.0**. See the LICENSE file for details.
