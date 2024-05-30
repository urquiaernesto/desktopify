Here's the entire content formatted as Markdown:

```markdown
<h1 align="center">Desktopify</h1>

## Convert Ubuntu Server for Raspberry Pi to a Desktop

Desktopify is a versatile script to convert [Ubuntu Server for the Raspberry Pi](https://ubuntu.com/download/raspberry-pi) to one of the official Ubuntu desktop flavours.

## Introduction

Desktopify helps in setting up a full Ubuntu Desktop environment on a Raspberry Pi. Initially created as a proof of concept, it has now evolved to support multiple Ubuntu desktop flavours.

## Installation

1. Download an [Ubuntu Server image for Raspberry Pi](https://ubuntu.com/download/raspberry-pi) and write it to an SDHC card.
2. Boot the Ubuntu Server SDHC on a Raspberry Pi 2, 3, or 4.
3. Log in to the Raspberry Pi using:
   - Username: `ubuntu`
   - Password: `ubuntu`
   - You will be prompted to change the password.
4. Clone the project:
   ```sh
   git clone https://github.com/wimpysworld/desktopify.git
   cd desktopify
   sudo ./desktopify --de ubuntu-mate
   ```

## Usage

```sh
./desktopify --de <desktop environment>

Available desktop environments:
  lubuntu
  kubuntu
  ubuntu
  ubuntu-budgie
  ubuntu-kylin
  ubuntu-mate
  ubuntu-studio
  xubuntu

You can also pass the optional --oem option which will run a setup wizard on the next boot.
Use --uninstall to remove the currently installed desktop environment.
```

## Features and Functions

### Install Desktop Environment

Installs the specified desktop environment:
```sh
sudo ./desktopify --de ubuntu-mate
```

### Uninstall Desktop Environment

Uninstalls the currently installed desktop environment:
```sh
sudo ./desktopify --uninstall
```

### OEM Setup

Runs an OEM setup wizard on the next boot:
```sh
sudo ./desktopify --de ubuntu-mate --oem
```

## Improvements and Achievements

- Installed GPIO utilities and libraries
- Enabled Bluetooth
- Made Network Manager the default backend
- Prevented low power WiFi mode
- Disabled overscan
- Enabled fkms driver
- Enabled boot splash
- Enabled Firefox hardware acceleration
- Created a snap package
- Supported desktop environments:
  - Kubuntu
  - Lubuntu
  - Ubuntu
  - Ubuntu Budgie
  - Ubuntu Kylin
  - Ubuntu MATE
  - Ubuntu Studio
  - Xubuntu
- Optimized Ubuntu MATE (Marco) window manager
- Enabled initial setup
- Prevented pointless re-installs
- Installed snaps
- Installed gpio tools

## Code Overview

### Main Functions

- `install_desktop_environment()`: Installs the specified desktop environment.
- `uninstall_desktop_environment()`: Uninstalls the currently installed desktop environment.
- `apply_tweaks()`: Applies specific tweaks for the installed desktop environment.
- `configure_network()`: Configures network settings and disables WiFi power saving.
- `display_menu()`: Displays a menu for selecting the desktop environment.

### Example Commands

Install Ubuntu MATE with OEM setup:
```sh
sudo ./desktopify --de ubuntu-mate --oem
```

Uninstall the current desktop environment:
```sh
sudo ./desktopify --uninstall
```

## Contribution

Feel free to contribute to the project by submitting issues or pull requests on [GitHub](https://github.com/wimpysworld/desktopify).

## License

This project is licensed under the MIT License - see the LICENSE file for details.
```

You can copy and paste this entire block into your README.md file on GitHub. If you need any further adjustments, let me know.
