# 🌐 LinguaPop — Floating Dictionary & Translator

> **Instantly understand words and phrases in English and your native language (Nepali, Hindi, and 100+ more) as you browse the web.**

LinguaPop is a lightweight, cross-browser extension built for **Microsoft Edge**, **Google Chrome**, and **Mozilla Firefox**. It empowers non-native English speakers to read fluently online without breaking their flow by copying and pasting words into new tabs.

---

## ✨ Features

- 📖 **Instant Floating Meaning on Selection**: Highlight any word or sentence on any website to immediately view its meaning.
- 🇳🇵 🇮🇳 **Bilingual Explanations**: Shows both the **English definition** (phonetics, parts of speech, examples, synonyms) and the translated meaning in **Nepali (नेपाली)**, **Hindi (हिन्दी)**, or any other chosen language.
- 🌍 **Works for Any Language**: Translate from any language into Nepali/Hindi/English or vice versa (auto-detects source text).
- 🔊 **Clear Pronunciation**: Built-in speech synthesis button allows you to hear the correct native pronunciation.
- ⚡ **Non-Intrusive Floating Icon**: By default, displays a subtle 📖 icon near your selected text. Clicking it opens the popup card so it never gets in the way when you are simply copying text.
- 📌 **Draggable & Pinnable**: Drag the popup card anywhere on your screen or pin it open while studying or reading articles.
- 🛡️ **Shadow DOM Isolation**: Webpage styling (fonts, CSS frameworks, colors) will never distort LinguaPop's card.
- 🆓 **100% Free & Zero Setup**: Uses public translation and dictionary endpoints out of the box. No accounts, API keys, or credit cards required.

---

## 🚀 How to Install

The extension is ready to use in your local workspace folder:
`C:\Users\Administrator\OneDrive - MSFT\Desktop\Samir Pariyar\Extensions`

### 1. Microsoft Edge
1. Open Edge and enter `edge://extensions/` in the address bar.
2. Turn on the **Developer mode** toggle (in the left-hand sidebar or bottom left).
3. Click the **Load unpacked** button at the top.
4. Browse to and select the folder:
   `C:\Users\Administrator\OneDrive - MSFT\Desktop\Samir Pariyar\Extensions`
5. Click **Select Folder**. The LinguaPop icon will appear in your Edge toolbar!

---

### 2. Google Chrome
1. Open Chrome and navigate to `chrome://extensions/`.
2. Toggle on **Developer mode** in the top-right corner.
3. Click the **Load unpacked** button in the top-left corner.
4. Select the folder:
   `C:\Users\Administrator\OneDrive - MSFT\Desktop\Samir Pariyar\Extensions`
5. Click **Select Folder**. Done!

---

### 3. Mozilla Firefox
1. Open Firefox and navigate to `about:debugging#/runtime/this-firefox`.
2. Click **Load Temporary Add-on...**.
3. In the file picker, select the `manifest.json` file inside:
   `C:\Users\Administrator\OneDrive - MSFT\Desktop\Samir Pariyar\Extensions\manifest.json`
4. LinguaPop will be loaded into Firefox.

---

## 🎯 How to Use

1. **Highlight Text on Any Page**:
   - Double-click a word or select a phrase on any website (e.g. Wikipedia, BBC, news, blogs).
   - A small purple floating icon (📖) will appear near the selected text.
   - Click the icon to view the full definition and translation card.

2. **Quick Language Switch**:
   - Inside the floating card, click **Nepali**, **Hindi**, or **English** chips, or choose any other language from the dropdown to translate instantly.

3. **Audio Speaker**:
   - Click the 🔊 speaker button in the header of the card to hear the pronunciation.

4. **Toolbar Search**:
   - Click the LinguaPop extension icon in your browser toolbar to type and search words directly without needing to be on a specific webpage.

5. **Change Preferences**:
   - Click the Settings gear in the toolbar popup or right-click the extension icon and select **Extension options**.
   - Change your primary language (default: Nepali), secondary language (default: Hindi), trigger mode (Floating button, Instant popup, or Alt/Ctrl + Select), or theme (Light / Dark).

---

## 📁 Project Structure

```
Extensions/
├── manifest.json              # Cross-browser Manifest V3 configuration
├── background.js              # Service worker handling translation & dictionary queries
├── content/
│   ├── content.js             # Selection listener & Shadow DOM popup interface
│   └── content.css            # Styles inside Shadow DOM
├── popup/
│   ├── popup.html             # Toolbar search popup UI
│   ├── popup.js               # Toolbar search & options logic
│   └── popup.css              # Toolbar UI styles
├── options/
│   ├── options.html           # Full settings page with live testing sandbox
│   ├── options.js             # Options storage and save logic
│   └── options.css            # Settings page styling
├── icons/                     # 16, 32, 48, 128 px PNG icons
└── README.md                  # Installation and usage instructions
```
