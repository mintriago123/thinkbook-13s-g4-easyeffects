# EasyEffects Profiles for Lenovo ThinkBook 13s G4 ARB

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/mintriago123/thinkbook-13s-g4-easyeffects?style=social)](https://github.com/mintriago123/thinkbook-13s-g4-easyeffects)
[![Realtek Version](https://img.shields.io/badge/Realtek-6.0.9430.1-blue)](https://download.lenovo.com/consumer/mobiles/g0t1077fmyebg9d0.exe)

English version | [Versión en Español](docs/README_ES.md)

Optimized audio profiles for EasyEffects based on the official Realtek audio driver for the Lenovo ThinkBook 13s G4 ARB.

> ⚠️ **DISCLAIMER**: These profiles are provided "as is" without warranty of any kind. Use at your own risk. The author is not responsible for any damage to your hardware, software, or hearing. Always use reasonable volume levels and test profiles at low volume first.

## 📋 Description

This repository contains audio profiles extracted from the official Realtek driver for the ThinkBook 13s G4 ARB, converted for use with EasyEffects on Linux. The profiles are optimized for different usage scenarios and replicate the audio experience of the official Windows driver.

## 🎵 Available Profiles

| Profile | File | Best For | Bass | Treble | Clarity |
|---------|------|----------|------|--------|----------|
| **Game** | `Thinkbook13s_Arb_Game.json` | Gaming, FPS | 🔊🔊🔊 | 🔊🔊🔊 | ⭐⭐⭐ |
| **Movie** | `Thinkbook13s_Arb_Movie.json` | Films, Series | 🔊🔊🔊🔊 | 🔊🔊 | ⭐⭐⭐⭐ |
| **Music** | `Thinkbook13s_Arb_Music.json` | Music listening | 🔊🔊🔊 | 🔊🔊🔊🔊 | ⭐⭐⭐⭐⭐ |
| **Universal** | `Thinkbook13s_Arb_Universal.json` | Daily use | 🔊🔊 | 🔊🔊 | ⭐⭐⭐ |
| **Voice** | `Thinkbook13s_Arb_Voice.json` | Video calls | 🔊 | 🔊🔊 | ⭐⭐⭐⭐⭐ |

## 💻 Compatibility

### Hardware
- **Model**: Lenovo ThinkBook 13s G4 ARB
- **Audio Chipset**: Realtek (PCI Subsystem ID: 17AA:3844)

### Software
- **Operating System**: Linux (any distribution)
- **Requirement**: EasyEffects installed
- **Based on**: Realtek Audio Driver 6.0.9430.1 for Windows 11 (64-bit)

## 📦 Installation

### Prerequisites

1. Install EasyEffects on your system:

```bash
# Ubuntu/Debian
sudo apt install easyeffects

# Fedora
sudo dnf install easyeffects

# Arch Linux
sudo pacman -S easyeffects
```

### Profile Installation

1. Clone this repository:
```bash
git clone https://github.com/mintriago123/thinkbook-13s-g4-easyeffects.git
cd thinkbook-13s-g4-easyeffects
```

2. Copy the profiles to the EasyEffects configuration folder:
```bash
mkdir -p ~/.config/easyeffects/output
cp profiles/*.json ~/.config/easyeffects/output/
```

3. Open EasyEffects and select the desired profile from the interface.

## 🔧 Usage

1. Launch EasyEffects
2. In the profiles menu, select the profile according to your activity:
   - **Game**: For gaming sessions with immersive audio
   - **Movie**: For enjoying movies with surround sound
   - **Music**: For Hi-Fi audio experience when listening to music
   - **Universal**: For daily use and multitasking
   - **Voice**: For video calls with optimized vocal clarity

## 📄 Original Configuration File

The [`drivers/DEV_0287_SUBSYS_17AA3844_PCI_SUBSYS_382717AA.xml`](drivers/DEV_0287_SUBSYS_17AA3844_PCI_SUBSYS_382717AA.xml) file contains the original configuration extracted from the Realtek driver that was used as the basis for creating these profiles.

## 📚 Original Driver Information

- **Driver Version**: Realtek 6.0.9430.1
- **Release Date**: July 25, 2025
- **Size**: 146.01 MB
- **Operating System**: Windows 11 (64-bit)
- **Type**: Recommended

### Official Links

- **Direct Download**: [Realtek Audio Driver](https://download.lenovo.com/consumer/mobiles/g0t1077fmyebg9d0.exe)
- **Support Page**: [Lenovo ThinkBook 13s G4 ARB - Drivers](https://pcsupport.lenovo.com/ec/es/products/laptops-and-netbooks/thinkbook-series/thinkbook-13s-g4-arb/downloads/driver-list/component?name=audio&id=3AA7F1C4-5B2A-453C-9CE2-B8FCDA8B69BA)

## 🛠️ Customization

Profiles can be edited according to your preferences:

1. Open EasyEffects
2. Load the profile you want to modify
3. Adjust the effect parameters to your liking
4. Save the profile with a new name or overwrite the existing one

## ⚠️ Notes

- These profiles were extracted from the official Windows driver and adapted for Linux
- Performance may vary depending on your hardware and software configuration
- It's recommended to try different profiles to find the one that best suits your needs

## ❓ FAQ

**Q: Do these profiles work on other Lenovo models?**  
A: They're optimized for ThinkBook 13s G4 ARB with Realtek ALC287, but may work on similar systems with the same audio chipset.

**Q: Can I use these with PulseEffects?**  
A: These are designed for EasyEffects (PipeWire). For PulseAudio/PulseEffects, some adjustments may be needed.

**Q: Will these damage my speakers?**  
A: No, these are safe profiles extracted from official drivers. However, always use reasonable volume levels to protect your hearing and hardware.

**Q: Why do I need to install EasyEffects?**  
A: EasyEffects is the audio processing tool that applies these profiles. It's the Linux equivalent of the Dolby Atmos software on Windows.

**Q: Can I modify these profiles?**  
A: Absolutely! These are starting points. Feel free to customize them to your preferences through the EasyEffects interface.

## 🤝 Contributions

Contributions are welcome. If you've created a custom profile or improved an existing one, feel free to submit a pull request.

## ⚖️ License & Legal

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

### Legal Disclaimer

These audio profiles were extracted from official Realtek drivers containing Dolby Atmos tuning. They are provided for educational and personal use under fair use principles for interoperability on Linux systems.

- **Dolby Atmos** is a trademark of Dolby Laboratories
- **Realtek** is a trademark of Realtek Semiconductor Corp.
- Not affiliated with Dolby, Realtek, or Lenovo

See [DISCLAIMER.md](DISCLAIMER.md) for full legal information.

## 📧 Support

If you encounter problems or have questions, please open an issue in this repository.

---

**Note**: This project is not officially affiliated with Lenovo or Realtek. The profiles are recreations based on the official driver to improve the audio experience on Linux.
