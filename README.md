# ChromaLayer

**Fix your laptop's washed-out display — no external monitor required.**

ChromaLayer is a lightweight Windows utility that gives you real-time control over your display's color and vibrancy, built specifically to solve the dull, low-saturation panels common on Intel-based laptops. Unlike GPU vendor tools that are locked to specific hardware, ChromaLayer works system-wide, applies instantly, and stays out of your way.

---

## ✨ Features

- **Real-time color adjustment** — Brightness, Contrast, Black Level, White Point, and Hue Shift, all with live preview (30ms debounce, no lag)
- **Vibrancy boost** — Recover the punch that stock Intel/laptop display drivers strip out
- **Presets** — Quick-switch profiles for **Gaming**, **Movie Night**, **Reading**, and **Night Mode**
- **System tray integration** — Runs quietly in the background, accessible with one click
- **Low overhead** — Built on the native Windows Magnification API, no GPU driver hacks or kernel-mode components
- **Game-safe** — Designed to avoid the anti-cheat and fullscreen-exclusive conflicts that plague overlay-based color tools

## 🖥️ Requirements

- Windows 10 or Windows 11
- Any GPU (Intel, AMD, NVIDIA) — no vendor-specific dependencies

## 📦 Installation

1. Download the latest release from the [Releases](../../releases) page
2. Run the installer (`ChromaLayerSetup.exe`)
3. Launch ChromaLayer — it will register itself to start automatically with Windows (can be disabled in Settings)
4. Adjust sliders or pick a preset from the tray icon

## 🚀 Quick Start

1. Right-click the ChromaLayer icon in your system tray
2. Choose a preset, or open the main window for manual control
3. Tweak sliders — changes apply live, no restart needed
4. Save your own custom preset for quick access later

## 🛠️ How It Works

ChromaLayer applies a 5×5 color transformation matrix system-wide using the **Windows Magnification API** (`MagSetFullscreenColorEffect`), combining vibrancy, color temperature, and tone adjustments in a single composited transform. Luminance calculations follow **ITU-R BT.709** weighting for accurate, natural-looking results.

Built with C# and WPF.

## 🗺️ Roadmap

- [ ] Display Clarity / sharpening (requires a DXGI-based rendering pipeline — planned for v2)
- [ ] Companion Chrome extension for browser-tab color matching
- [ ] Additional presets and per-app profiles

## ⚠️ Known Limitations

- Sharpening/clarity adjustments are not currently supported (a limitation of the Magnification API) — planned for a future DXGI-based v2
- Free trial with paid unlock for full feature access (see app for details)

## 🤝 Contributing

Issues and feature requests are welcome — please open an [Issue](../../issues) describing the bug or suggestion, along with your Windows version and GPU.

## 📄 License

*(Add your license here — e.g. MIT, Proprietary, etc.)*

## 💬 Support / Feedback

Found a bug or have an idea? Open an issue, or reach out via [your contact/socials here].

---

<p align="center">Made for anyone stuck staring at a washed-out laptop screen.</p>
