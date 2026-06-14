<div align="center">



# MaLauncher

### A Minecraft: Java Edition launcher for iOS

![Platform](https://img.shields.io/badge/platform-iOS%2014%2B-blue?style=flat-square)
![License](https://img.shields.io/github/license/TomaTheLoser/MaLauncher?style=flat-square)
![Release](https://img.shields.io/github/v/release/TomaTheLoser/MaLauncher?style=flat-square)
![Downloads](https://img.shields.io/github/downloads/TomaTheLoser/MaLauncher/total?style=flat-square)

</div>

---

## ✨ Features

| Feature | Description |
|---|---|
| 🎮 **Full Minecraft Java** | Run Minecraft: Java Edition natively on your iPhone or iPad |
| 👤 **Account flexibility** | Play with a local offline account or sign in with your Microsoft account |
| ⚡ **Automatic JIT** | JIT compiles automatically on jailbroken devices — no external tools needed |
| 🖥️ **Metal rendering** | ANGLE renderer uses Apple's Metal API for smooth, native GPU performance |
| 🧩 **Mod support** | Full support for Forge, Fabric, and OptiFine |
| 📦 **No PC required** | Install directly on your device with eSign or any IPA installer |

---

## 📋 Requirements

### Jailbroken devices ✅
- iPhone or iPad running **iOS 14.0 or later**
- Any jailbreak that supports rootless (palera1n recommended)
- eSign or any IPA installer app

### Non-jailbroken devices ⚠️
- iPhone or iPad running **iOS 14.0 or later**
- [AltStore](https://altstore.io) installed on your device
- AltServer running on a computer on the same Wi-Fi network to enable JIT before each launch

---

## 📥 Installation

### Jailbroken (Recommended)

1. Go to [**Releases**](../../releases/latest) and download the latest `.ipa`
2. Open it with **eSign** or your preferred IPA installer
3. Trust the app if prompted in **Settings → General → VPN & Device Management**
4. Launch **MaLauncher** — JIT is enabled automatically
5. Choose or create an account and start playing

### Non-jailbroken

1. Install [AltStore](https://altstore.io) following their official guide
2. Download the latest `.ipa` from [**Releases**](../../releases/latest)
3. Open the `.ipa` with AltStore to install
4. Before launching, make sure **AltServer is running** on your computer on the same Wi-Fi
5. Launch **MaLauncher** — AltStore will enable JIT automatically

---

## 🎮 Supported Minecraft Versions

| Version Range | Loader Support | Status |
|---|---|---|
| 1.7.10 – 1.12.2 | Forge | ✅ Fully supported |
| 1.13 – 1.16.5 | Forge, Fabric | ✅ Fully supported |
| 1.17 – 1.20.4 | Forge, Fabric, OptiFine | ✅ Fully supported |
| 1.20.5+ | Fabric | ⚠️ May have issues |

---

## 🖥️ Recommended Renderers

Choosing the right renderer makes a big difference in performance and compatibility.

| Renderer | Best For | Notes |
|---|---|---|
| **ANGLE** | 1.17 and above | Uses Apple Metal natively — best performance and compatibility for modern versions |
| **Holy GL4ES 1.1.5** | 1.16 and below | Best choice for older versions |
| **Holy (GL4ES)** | 1.12.2 and below | Fallback option for very old versions |

> 💡 **Tip:** If you experience graphical glitches, try switching renderers first before anything else.

---

## ⚠️ Known Issues

- **Performance mods** that replace the rendering pipeline (e.g. Sodium, ImmediatelyFast) are not compatible — use **OptiFine** instead for performance improvements
- **TrollStore** is not supported on iOS 16.7.x (except the specific RC build `20H18`)
- Some very new Minecraft versions (1.20.5+) may have compatibility issues

---

## ❓ FAQ

**Q: Do I need to pay for Minecraft to use this?**
A: MaLauncher supports both local offline accounts and purchased Microsoft accounts. To access online servers and your purchased content, a valid Microsoft account is required.

**Q: Will this work on my non-jailbroken iPhone?**
A: Yes, but you'll need AltStore and AltServer running on a computer on the same Wi-Fi each time you launch the game to enable JIT.

**Q: Which Minecraft version should I play for best performance?**
A: 1.12.2 with Forge + OptiFine is the most stable and performant option on iOS. Modern versions (1.17+) work well too with the ANGLE renderer.

**Q: Can I use shaders?**
A: Yes — OptiFine shaders work on compatible versions. Start with lightweight shader packs for best results on older devices.

**Q: Why does the game need JIT?**
A: Minecraft: Java Edition uses a JVM that requires Just-In-Time compilation to run at acceptable speeds. iOS restricts JIT by default, which is why jailbroken devices have the smoothest experience.

---

## 📜 Credits & Legal

MaLauncher is built on top of open source components. The following projects and their respective authors made this possible:

- **PojavLauncher iOS** by the [PojavLauncher Team](https://github.com/PojavLauncherTeam/PojavLauncher_iOS) — the original iOS Minecraft Java launcher this project is based on
- [Caciocavallo](https://github.com/PojavLauncherTeam/caciocavallo) — GNU GPLv2
- [Boardwalk](https://github.com/zhuowei/Boardwalk) — Apache 2.0
- [GL4ES](https://github.com/ptitSeb/gl4es) — MIT
- [MetalANGLE](https://github.com/khanhduytran0/metalangle) — BSD 2.0
- [MoltenVK](https://github.com/KhronosGroup/MoltenVK) — Apache 2.0
- [openal-soft](https://github.com/kcat/openal-soft) — LGPLv2
- [LWJGL3](https://github.com/PojavLauncherTeam/lwjgl3) — BSD-3
- [AltKit](https://github.com/rileytestut/AltKit)
- [UnzipKit](https://github.com/abbeycode/UnzipKit) — BSD-2
- [DyldDeNeuralyzer](https://github.com/xpn/DyldDeNeuralyzer)
- [fishhook](https://github.com/khanhduytran0/fishhook) — BSD-3
- [Mesa 3D Graphics Library](https://gitlab.freedesktop.org/mesa/mesa) — MIT

This project is licensed under the **GNU General Public License v3.0**. See [LICENSE](LICENSE) for details.
