<div align="center">

# ⛏️ MaLauncher

### Minecraft: Java Edition — running natively on iOS.

![Platform](https://img.shields.io/badge/platform-iOS%2014%2B-2E7D32?style=for-the-badge)
![License](https://img.shields.io/github/license/TomaTheLoser/MaLauncher?style=for-the-badge&color=8B4513)
![Release](https://img.shields.io/github/v/release/TomaTheLoser/MaLauncher?style=for-the-badge&color=D84315)
![Downloads](https://img.shields.io/github/downloads/TomaTheLoser/MaLauncher/total?style=for-the-badge&color=2E7D32)

</div>

▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰

MaLauncher is built on PojavLauncher iOS, with ongoing fixes and additional features layered on top.

## 🟩 What It Does

**Runs without a computer, even without JIT.**
Jailbroken devices get JIT automatically. Non-jailbroken devices can use AltStore + AltServer to enable it. But if neither is available, MaLauncher can still run Minecraft 1.16.5 and below using a zero-assembly Java 8 runtime — no JIT, no computer, no AltServer. Just install and play.

**Java runtimes, managed in-app.**
Browse and download JREs straight from the Manage Runtimes screen — no Safari, no file manager, no manually dropping folders into place. You can also install more than one build of the same Java version side-by-side (e.g. a standard JIT build next to a zero-assembly build) and pick exactly which one each profile uses.

**Renderer that picks itself.**
GL4ES for 1.16.5 and below, ANGLE (Apple Metal) for 1.17 and up — chosen automatically based on the version you're launching. Override it manually per-profile if you want to mess with it, but you shouldn't need to.

**Mods just work.**
Forge, Fabric, and OptiFine are all supported across the version ranges below.

**Accounts, your way.**
Local offline profiles for quick testing, or sign in with Microsoft for online play and your purchased content.

▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰

## 🟧 Requirements & Install

### Jailbroken
- iOS 14.0+, any rootless jailbreak (palera1n recommended)
- eSign or any IPA installer

1. Grab the latest `.ipa` from [**Releases**](../../releases/latest)
2. Install with eSign (or your installer of choice)
3. Trust it in **Settings → General → VPN & Device Management** if prompted
4. Open MaLauncher — JIT is already on. Play.

### Non-jailbroken
- iOS 14.0+, [AltStore](https://altstore.io) installed
- AltServer running on a computer on the same Wi-Fi to enable JIT each launch

1. Set up AltStore following their guide
2. Install the latest `.ipa` from [**Releases**](../../releases/latest) through AltStore
3. Keep AltServer running on your computer before launching
4. Open MaLauncher — AltStore handles JIT for you

### No JIT available at all
Stuck without a jailbreak or a second device to run AltServer? You're not locked out.

1. In **Manage Runtimes**, download the **zero-assembly Java 8** build
2. Set it as the runtime for any profile running **Minecraft 1.16.5 or older**
3. Launch — no JIT required

▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰

## 🟦 Supported Versions

| Version Range | Loaders | Status |
|---|---|---|
| 1.7.10 – 1.12.2 | Forge | ✅ Fully supported |
| 1.13 – 1.16.5 | Forge, Fabric | ✅ Fully supported |
| 1.17 – 1.20.4 | Forge, Fabric, OptiFine | ✅ Fully supported |
| 1.20.5+ | Fabric | ⚠️ May have issues |

▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰

## 🟥 Known Issues

- Performance mods that swap out the rendering pipeline (Sodium, ImmediatelyFast) aren't compatible — use **OptiFine** instead
- TrollStore isn't supported on iOS 16.7.x, except the `20H18` RC build
- 1.20.5+ may have rough edges

▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰

## 🟫 FAQ

**Do I need to buy Minecraft?**
Only if you want online servers or your purchased content. Offline play works with a local account, no purchase needed.

**Will this run on a non-jailbroken iPhone with no second device for AltServer?**
Yes, for 1.16.5 and below — use the zero-assembly Java 8 runtime described above. For 1.17+, you'll need either a jailbreak or AltServer to get JIT.

**Best version for performance?**
1.12.2 with Forge + OptiFine is the most stable combo on iOS hardware. 1.17+ runs well too, with ANGLE doing the heavy lifting on Metal.

**Shaders?**
Yes, via OptiFine. Start light on older devices.

**Why does this even need JIT?**
The Java JVM leans on Just-In-Time compilation for speed, and iOS blocks JIT by default outside specific exceptions (jailbreak, AltServer-assisted debug mode). The zero-assembly runtime sidesteps this entirely by not needing JIT — slower, but it runs anywhere.

▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰▰

## ⬛ Credits & Legal

Built on the work of:

- **PojavLauncher iOS** — [PojavLauncher Team](https://github.com/PojavLauncherTeam/PojavLauncher_iOS), the original codebase this project is based on
- [Caciocavallo](https://github.com/PojavLauncherTeam/caciocavallo) — GPLv2
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

Licensed under **GPLv3**. See [LICENSE](LICENSE).
