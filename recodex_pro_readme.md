# ⚡ ReCodeX Pro — File Combiner & Extractor

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](#)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white)](#)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](#)
[![Client--Side Only](https://img.shields.io/badge/Privacy-100%25_Client--Side-green)](#)

**ReCodeX Pro** is a zero-dependency, single-file browser utility designed to bundle multiple source files into a single structured text file and reverse-split them back with 100% file integrity.

It is particularly useful for developer workflows, AI prompt engineering (feeding entire project codebases into LLMs like ChatGPT, Claude, or Gemini), code archiving, and offline file bundling.

---

## ✨ Features

- **📦 Batch File Compilation**: Drag & drop multiple source files or scripts to merge them into a single structured file.
- **🔄 Reverse Splitter (Extraction)**: Re-upload any compiled ReCodeX file to automatically parse, split, and extract the individual files back to your computer.
- **🤖 Ideal for AI/LLM Workflows**: Converts multi-file software projects into a single formatted text block with clear file delimiters—perfect for large context window AI prompts.
- **🔒 100% Client-Side & Private**: Runs completely inside your web browser. Your files and code never touch an external server or API.
- **⚡ Zero Setup**: Packed in a standalone HTML file. No `npm install`, Node.js server, or build step required.
- **🎨 Modern Responsive UI**: Styled with Tailwind CSS, featuring drag-and-drop upload areas, code preview modals, and one-click clipboard copying.

---

## 🛠️ How It Works

ReCodeX Pro uses clean, human-readable structural comments to encapsulate each file during compilation:

```javascript
/* START_FILE: src/index.js */
console.log("Hello, ReCodeX!");
/* END_FILE: src/index.js */

/* START_FILE: src/styles.css */
body { background: #1E2328; }
/* END_FILE: src/styles.css */
```

When reversing the process, the built-in parser reads these delimiter tags using regular expressions, isolates the content, and generates native browser downloads for each original file.

---

## 🚀 Quick Start

### 1. Run Locally
Because ReCodeX Pro is a single-file application, you don't need any complex installation:

1. Clone or download this repository:
   ```bash
   git clone https://github.com/your-username/recodex-pro.git
   ```
2. Open `reocdex.html` directly in any modern web browser (Chrome, Firefox, Edge, Safari).

### 2. Deploy to GitHub Pages
1. Push `reocdex.html` to your repository.
2. Go to **Settings > Pages** in your GitHub repository.
3. Select `main` branch as the source and save.
4. Rename `reocdex.html` to `index.html` if you want it served as your primary landing page.

---

## 💡 Typical Use Cases

| Use Case | Description |
| :--- | :--- |
| **AI / LLM Prompts** | Bundle an entire frontend or backend project into one master text snippet to paste into ChatGPT or Claude for code audits, debugging, or refactoring. |
| **Code Audits & Review** | Combine scattered module files into one document for quick searching or printing. |
| **Source Backup** | Package source scripts into a lightweight plain-text archive without requiring zip utilities. |
| **Project Unbundling** | Receive a combined file from an AI response or teammate and unpack it into individual files with a single click. |

---

## 🧰 Tech Stack

- **Markup & Layout**: HTML5
- **Styling**: Tailwind CSS (via CDN)
- **Scripting**: Vanilla JavaScript (ES6+ Async/Await, Blob API, RegExp)
- **Archive Handling**: JSZip library (included via CDN for batch ZIP downloads)

---

## 📁 Repository Structure

```
.
├── reocdex.html      # Complete application (HTML, CSS, JS)
└── README.md         # Project documentation
```

---

## 📄 License

This project is licensed under the **MIT License**. Feel free to use, modify, and distribute it for personal or commercial projects.