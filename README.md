# 🎮 fortnite-auto-building-pro

[![tool](https://img.shields.io/badge/tool-MIT-green?style=flat-square) ![Version](https://img.shields.io/badge/Version-1.2.0-blue?style=flat-square) ![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey?style=flat-square) ![Python](https://img.shields.io/badge/Python-3.11%2B-3776AB?style=flat-square&logo=python&logoColor=white) ![Stars](https://img.shields.io/github/stars/oliverkumar-devt7/fortnite-auto-building-pro?style=flat-square) ![Last Commit](https://img.shields.io/github/last-commit/oliverkumar-devt7/fortnite-auto-building-pro?style=flat-square)

Fortnite-auto-building — — pixel detection, crosshair overlay, configurable settings

## 📥 Download

[![Download Latest](https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge&logo=github)](../../releases/latest)

1. Download the latest release from the link above
2. Extract the archive (WinRAR / 7-Zip)
3. Run `python main.py` (or see Usage below)
4. Configure settings in `config.yaml`

## Getting Started

First, make sure you have Python 3.11 or later installed.

1. Clone the repository: `git clone https://github.com/oliverkumar-devt7/fortnite-auto-building-pro.git`
2. Navigate to the project directory: `cd fortnite-auto-building-pro`
3. Install the required packages: `pip install -r requirements.txt`

## Basic Usage

To run the application:

1. Make sure Fortnite is running.
2. Execute the main script: `python main.py`
3. The overlay should appear. Tweak settings in `config.yaml` as needed.

## Config

The `config.yaml` file lets you customize the utility. Here's an example:

```yaml
# Overlay settings
overlay_color: "red"
crosshair_size: 15
crosshair_thickness: 2

# Pixel detection
pixel_threshold: 150
detection_region:
 x1: 500
 y1: 300
 x2: 700
 y2: 500

# Hotkeys
build_hotkey: "f"
# Monitor settings
monitor_id: 0
```

## Highlights

* **Screen Analysis:** Analyze regions of your screen.
* **Overlay:** Displays an on-screen overlay.
* **Crosshair:** Puts a customizable crosshair on the screen.
* **Pixel Detection:** Detects specific pixel values within a region.
* **Hotkey Automation:** Automates actions based on hotkey presses.
* **Configuration:** All settings are configurable.

## FAQ

<details>
<summary>The overlay isn't showing up. What do I do?</summary>
Make sure you've installed all requirements. Try running as admin.
</details>

<details>
<summary>How do I find the right pixel threshold?</summary>
Use the `monitor.py` script to inspect pixel values in real-time. Adjust the threshold in `config.yaml` until you get desired results.
</details>

<details>
<summary>Can I use different hotkeys?</summary>
Yep! Change the hotkey assignments in the `config.yaml` file.
</details>

## Troubleshooting

* **Problem:** The tool isn't detecting pixels correctly.
 * **Solution:** Adjust the `pixel_threshold` in `config.yaml`. Ensure the `detection_region` is correct.

* **Problem:** The overlay flickers.
 * **Solution:** Try different `overlay_color` values. Reduce crosshair thickness.

* **Problem:** Hotkeys aren't working.
 * **Solution:** Make sure Fortnite is focused. Ensure the hotkeys don't conflict with other applications.

---

🛠 Built with Python | Open Source