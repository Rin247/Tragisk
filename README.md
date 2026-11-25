# Tragisk — Modern Android Root Manager & System Suite

Tragisk is an advanced Android root management and system customization suite based on Magisk. Combining MagiskSU, Zygisk code injection, MagiskBoot boot image patching, and a modern Jetpack Compose manager application (`app/`), Tragisk gives power users and developers complete, transparent control over their Android devices.

---

## ⚡ Key Features & Module Breakdown

### 🔓 MagiskSU & Superuser Gateway (`su`)
- **Current**: Fine-grained root permission granting, per-app access prompts, root access logging, and PIN security lock.
- **Planned / Roadmap**: Temporary root access timers, root access profiles, and multi-user isolation controls.

### 💉 Zygisk Code Injection (`zygisk`)
- **Current**: Native Zygote process entry point injection, module hook API, and isolated process sandboxing.
- **Planned / Roadmap**: Next-gen hook engine optimizations, lower memory overhead, and advanced anti-tamper isolation options.

### 📦 Module Manager & Systemless Overlays (`modules`)
- **Current**: Systemless module installation, active module toggle list, overlay mount manager, and module repository support.
- **Planned / Roadmap**: WebDAV module sync, module compatibility verification, and automatic update checker.

### 🛠️ MagiskBoot & Image Patching (`boot`)
- **Current**: Boot image (`boot.img` / `init_boot.img`) patching, kernel unpack/repack, and ramdisk modification.
- **Planned / Roadmap**: Automated APatch / KernelSU compatibility mode, AVB (Android Verified Boot) header patcher, and AB partition OTA survival script.

---

## 🏗️ Architecture & Technology Stack

- **Manager App**: Kotlin, Jetpack Compose, Material 3 (minSdk 33, targetSdk 37).
- **Native Suite**: C++20, Rust, POSIX shell daemon (`magiskd`).
- **Build System**: Android NDK r27+, Rust cargo, Python build scripts.
- **Licensing**: GPL-3.0.

---

## 🛠️ Building & Running

### Prerequisites
- **Android Studio** (2026.2.2+) / NDK r27+
- **Rust toolchain** (`cargo`)
- **JDK 25**

### Build Commands

```bash
# Build Manager APK & Native Binaries
./gradlew assembleDebug
```

---

## 📜 License

Tragisk is released under the **GNU General Public License v3.0** (GPL-3.0). See [`LICENSE`](LICENSE) for details.
