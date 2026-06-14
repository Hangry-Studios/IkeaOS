# ikeaOS

ikeaOS is a minimal operating system built using Debian Live-Build. It features the KDE Plasma desktop environment and the Firefox web browser.

## Core Packages

The installation includes only the following packages above the standard Debian base system:

*   **Desktop Environment:** `kde-plasma-desktop`
*   **Display Manager:** `sddm`
*   **Web Browser:** `firefox-esr`

## Installation

1. Download the ISO image.
2. Flash the image to a USB drive.
3. Boot from the USB drive and complete the system installation.

## Building from Source

To build ikeaOS using `live-build` on a Debian environment, execute the following commands:

```bash
# Initialize live-build configuration
lb config

# Define package list
echo "kde-plasma-desktop sddm firefox-esr" > config/package-lists/ikeaos.list.chroot

# Build the ISO image
sudo lb build
