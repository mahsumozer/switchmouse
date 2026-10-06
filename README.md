<p align="center"><img src="icon.png" width="96" alt=""></p>

<h1 align="center">SwitchMouse</h1>
<p align="center">One mouse and keyboard for your Mac and your Windows PC.</p>

<p align="center"><a href="https://github.com/mahsumozer/switchmouse/releases/latest"><b>⬇ Download the latest release</b></a></p>

---

Push the cursor past the edge of your screen and it continues on the other computer, keyboard included. Press **Ctrl + Alt + M** (⌃⌥M on Mac) to switch at any time.

- **Simple** – pick *Share this mouse* on the computer the mouse is plugged into and *Connect* on the other; they find each other on the local network.
- **Secure** – paired once with a 6-digit code (CPace PAKE), then every connection is mutually authenticated, end-to-end encrypted TLS 1.3. Unpaired devices can't send or receive input.
- **Fast** – a few bytes per mouse event over a direct LAN connection.
- Per-display edges for multi-monitor setups, text clipboard sharing, optional Cmd ↔ Ctrl swap.
- On macOS it lives in the menu bar.

> **Early preview.** The interface is in Turkish for now.

## Install

| | File |
|---|---|
| macOS 12+ (Apple Silicon & Intel) | `SwitchMouse-<version>-macOS.dmg` |
| Windows 10/11 (most PCs) | `SwitchMouse-<version>-Windows-x64.exe` |
| Windows on ARM | `SwitchMouse-<version>-Windows-ARM64.exe` |

**macOS** – open the DMG and drag SwitchMouse to Applications. The build is signed but not yet notarized, so the first launch is blocked: go to *System Settings → Privacy & Security* and click *Open Anyway*. Then grant *Accessibility* access when asked; it is needed to capture and move the mouse.

**Windows** – run the exe. If SmartScreen appears, choose *More info → Run anyway*. Allow it on *private networks* when the firewall asks. Requires WebView2, which ships with Windows 10 and 11.

## Pairing

1. On the computer with the mouse and keyboard: **Fareyi paylaş** (Share this mouse). Mark which side the other screen is on.
2. On the other computer: **Bağlan** (Connect), then pick the computer from the list or type its IP address.
3. Enter the 6-digit code shown on the first computer. That's it – from then on they connect automatically.

**Troubleshooting:** both computers must be on the same network. A VPN with a kill switch (e.g. Mullvad lockdown mode) blocks the connection unless *local network sharing* is enabled in the VPN.

Verify downloads against `SHA256SUMS.txt` attached to each release.

---

### Türkçe

Fareyi ekran kenarına itince imleç diğer bilgisayarda devam eder; klavye de onunla gider. **Ctrl + Alt + M** (Mac'te ⌃⌥M) ile istediğiniz an geçiş yapabilirsiniz. [Son sürümü indirin](https://github.com/mahsumozer/switchmouse/releases/latest), fare ve klavyenin bağlı olduğu bilgisayarda **Fareyi paylaş**'ı, diğerinde **Bağlan**'ı seçin ve ekranda çıkan 6 haneli kodu girin.
