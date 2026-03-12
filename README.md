# Lynea OS - Alpha

<img src="images/lynea_logo.png" alt="Lynea Logo" width="342px">

Lynea is a daily-usable, technically-installed phone OS project.  
This repository contains device-specific source code and shared generic code for Lynea Alpha.

---

## Repository Structure

- `common/` → Generic code used across all devices
  - `tools/` → LYSU, CLI utilities
  - `scripts/` → Generic helper scripts
  - `docs/` → General documentation

- `devices/` → Device-specific source code
  - `gale/` → Xiaomi Redmi 13C
    - `bootloader/` → Device bootloader sources
    - `kernel/` → Device kernel sources
    - `rootfs/` → Device root filesystem
  - `a01core/` → Samsung Galaxy A01 Core
  - `oriole/` → Google Pixel 6

- `images/` → Logos and images
  - `lynea_logo.png`

---

## License

- Kernel / Bootloader: GPLv3  
- Tools / Scripts / Generic code: MIT  

---

## Installation

Lynea Alpha is intended for technical users only.

1. Open the relevant device folder (`devices/XXX/`).  
2. Follow bootloader, kernel, and rootfs installation instructions provided in the folder README or documentation.  
3. Generic tools in `common/` can be reused across devices.

---

## Notes

- Each device’s sources are **isolated** to prevent conflicts between different kernel or bootloader patches.  
- Generic modules are **common across devices** and can be reused.  
- Logo and images are included for demonstration purposes in the alpha version.
