# Installation Guide

## Requirements

- **Python 3.8+**
- **Google Chrome** browser installed
- **ChromeDriver** matching your Chrome version (usually managed automatically by newer Selenium versions).
- Standard internet connection for web scraping.

## Setup & Installation

1. **Clone/Download the Repository**
   Ensure you have the `Bookmark` directory downloaded to your local machine.

2. **Open Terminal**
   Navigate to the `Bookmark` folder.
   ```bash
   cd path/to/Bookmark
   ```

3. **Install Dependencies**
   Install the required Python packages using pip.
   ```bash
   pip install selenium pandas openpyxl
   ```

## Configuration

Before running the application, you must configure your credentials and target constraints.

1. Open `dd_msg_sender.py` in your preferred text editor.
2. Locate the **CONFIGURATION** section.
3. Update the credentials:
   ```python
   USERNAME = "YourDamaDamUsername"
   PASSWORD = "YourDamaDamPassword"
   ```
4. Customize target rows:
   ```python
   START_ROW = 4  # 0-based index where script starts reading Excel
   END_ROW = 6    # 0-based index where script stops
   ```

## Troubleshooting & Common Errors

- **`ModuleNotFoundError: No module named 'selenium'`**
  - **Fix:** Run `pip install selenium`
- **`SessionNotCreatedException: Message: session not created: This version of ChromeDriver only supports Chrome version XX`**
  - **Fix:** Update your Google Chrome browser to the latest version, or manually download the matching ChromeDriver and place it in your system PATH.
- **Bot gets stuck or fails to find text area**
  - **Fix:** React interfaces update dynamically. Check your internet connection speed. If the page loads too slowly, increase the `time.sleep()` delays inside the `MessageSender` class.

---

## 👨‍💻 Credits

**By OutLawZ™**

Website: https://www.brandex.pk

Need custom automation, AI tools, workflow systems, dashboards, integrations, scraping tools, content automation, or business process automation?

Contact:

📧 Email: net2tara@gmail.com
🌐 Website: https://www.brandex.pk
📘 Facebook: Coming Soon
📸 Instagram: Coming Soon
▶️ YouTube: Coming Soon

---
Made with ❤️ by OutLawZ™
