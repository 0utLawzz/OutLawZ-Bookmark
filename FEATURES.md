# Features

## Main Features

- **Automated Authentication**: Logs into the target social media platform using defined credentials automatically on script execution.
- **Bulk Messaging**: Traverses a predefined list of targets and automatically posts customized comments on their profiles.
- **Database Synchronization**: Directly reads from and writes to `Final_Cleaned.xlsx`.

## Automation Features

- **Intelligent Resumption**: Skips previously processed rows by checking the `Status` column for existing entries, meaning the script can be safely restarted if it crashes.
- **Dynamic Element Searching**: Uses multiple CSS selectors in a fallback loop to identify posts and text areas. If UI changes slightly, the bot attempts alternative DOM paths.
- **React Input Dispatch**: Native browser `click` and `send_keys` often fail on React/Vue textareas. This script uses JavaScript event dispatchers (`Event('input')` and `Event('change')`) to mimic actual human typing, bypassing client-side validation blockers.

## Hidden Features

- **Row Slicing**: Allows processing a specific subsection of the Excel list (using `START_ROW` and `END_ROW`) without altering the source spreadsheet.
- **Lenient Verification**: If the bot is unsure if a message sent properly due to lag, it scans the DOM for the first 10 characters of the payload to verify delivery without throwing unnecessary errors.

## Limitations

- Currently hardcoded for a single platform (DamaDam).
- Requires a graphical browser session (headless mode is currently disabled for debugging).

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
