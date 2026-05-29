# 🎯 KeyTap Pro v4.0.0

KeyTap Pro is a portable productivity suite built using **AutoHotkey v2**. Initially designed as a simple auto-incrementing invoice generator, it has evolved into a fully featured automation tool equipped with dynamic macro mapping, an automated VAT calculator, and an intuitive tabbed user interface.

With KeyTap Pro, you can eliminate repetitive typing, streamline financial calculations, and manage your custom hotkeys on the fly without ever touching a line of code.

---

## ✨ Key Features

* **Smart Invoice Generator (`Alt + F9`):** Instantly types a structured invoice number (Prefix + 7-Digit Sequential Number + Suffix). The counter automatically increments by 1 and updates locally.
* **Dynamic Custom Text Hotkeys:** Easily map your own shortcuts (e.g., `Alt+A`, `Ctrl+Shift+D`) to custom text templates using the interactive built-in Management Panel.
* **Automated VAT Deductor (`Alt + V`):** Highlight any gross amount containing 12% VAT, press the shortcut, and watch it instantly recalculate and replace the text with the Net Amount.
* **Completely Portable:** No installation required. Runs directly from a USB drive, shared folder, or your local directory. All settings are saved locally in a `settings.ini` file.

---

## 🛠️ Global System Shortcuts

| Shortcut | Action | Description |
| :--- | :--- | :--- |
| `Alt + F9` | **Generate Invoice** | Automatically types the next invoice string and increments the counter. |
| `Alt + F10` | **Open Manager** | Launches the main graphical interface control panel. |
| `Alt + V` | **Calculate Net VAT** | Extracts, processes, and deducts 12% VAT from selected text. |

---

## 🚀 How to Install & Run

### Method 1: Using the Pre-compiled Executable (Recommended)
1. Go to the [Releases](https://github.com/JeromRequillo/KeyTap-Pro/releases) page.
2. Download the `KeyTap_Pro_v4.1.exe` binary.
3. Place it in your preferred folder and double-click to run!

### Method 2: Running from Source
1. Ensure you have [AutoHotkey v2](https://www.autohotkey.com/) installed on your machine.
2. Clone or download this repository.
3. Run the `KeyTap_Pro.ahk` script file.

> 💡 **Tip:** To make KeyTap Pro start automatically when Windows boots, press `Win + R`, type `shell:startup`, and place a shortcut of the executable or script inside that folder.

---

## 📖 User Guide

### 1. Invoice Configuration
* Set your desired **Prefix** (e.g., `AAPI`), starting **Next Number** (e.g., `1`), and **Suffix** (e.g., `S`).
* Check the real-time **Live Preview** box before saving.
* Click **Reset** to quickly return the counter value to zero.

### 2. Custom Shortcuts Management
* Use the standard AHK modifiers to register keys in the list view:
    * `!` = Alt
    * `^` = Ctrl
    * `+` = Shift
* *Example:* Entering `!A` in the Shortcut Key field and `Hello World` in the output field will send "Hello World" every time you press `Alt + A`.

### 3. Automated VAT Calculator
* Highlight **only** the numerical digits and commas (e.g., `1,500.00`). Do not include currency symbols like `₱` or `$`.
* Press `Alt + V` to update the text.
* If you accidentally miscalculate or overwrite something, simply press `Ctrl + Z` in your text editor to undo.

---

## 📂 File Structure

```text
📂 KeyTap Pro/
├── 📄 KeyTap_Pro_v4.1.exe   # Compiled Standalone Application
├── 📄 KeyTap_Pro.ahk        # Source Code (AHK v2)
├── 📄 settings.ini          # Configuration File (Auto-generated)
└── 📄 README.md             # Project Documentation
