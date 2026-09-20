# 📖 Markdown Viewer & Reader

An elegant, single-file browser utility for rendering Markdown files and text with a warm, editorial manuscript aesthetic. 

Built with vanilla JavaScript, custom CSS, and `marked.js`, this zero-setup tool allows you to easily inspect, upload, or paste Markdown content directly within your web browser.

---

## ✨ Features

- **📄 Local File Upload**: Load any `.md` file from your computer to parse and render formatted HTML instantly.
- **✍️ Raw Text Input**: Paste or edit raw Markdown text directly in the interactive textarea editor.
- **🎨 Manuscript & Editorial Typography**: Styled with a warm paper palette and typography (`Fraunces` for headings, `Inter` for tables/body, and `IBM Plex Mono` for code blocks and UI controls).
- **🏷️ Dynamic Document Header**: Automatically displays the active file name or flags pasted content.
- **⚡ Client-Side Processing**: Runs completely inside your browser. No data or text is ever transmitted to an external server.
- **📱 Responsive & Accessible**: Styled with custom media queries for mobile viewing and support for high-contrast/reduced-motion preferences.

---

## 🛠️ How It Works

The viewer leverages client-side file reading and the [Marked.js](https://marked.js.org/) parsing library:

1. **File Input**: Selecting a file invokes `loadMarkdownFile()`, which reads the text stream using `file.text()` and parses it to HTML.
2. **Text Input**: Clicking **Render Markdown** parses the raw text inside the editor textarea into formatted HTML.
3. **Default Content**: On initial page load, the script attempts to fetch a local file named `level2_game_story.md` as sample content if hosted on a web server.

---

## 🚀 Quick Start

### Option 1: Direct File Opening
Since the application is packaged as a single static file, you can run it directly:
1. Save or download `md_file_viewer.html`.
2. Double-click `md_file_viewer.html` (or right-click and open with your preferred browser).

### Option 2: Local HTTP Server (Recommended for default file fetching)
To allow the application to fetch default sample files without CORS restrictions:

Using Python:
```bash
python3 -m http.server 8000
```
Then navigate to `http://localhost:8000/md_file_viewer.html` in your browser.

Using Node.js (`npx`):
```bash
npx serve .
```

---

## 🧰 Tech Stack

- **Markup & Layout**: HTML5
- **Styling**: Custom CSS3 (CSS Variables, Flexbox, CSS Grid)
- **Scripting**: Vanilla JavaScript (ES6+ Async/Await, Fetch API, FileReader API)
- **Markdown Engine**: [Marked.js](https://cdn.jsdelivr.net/npm/marked/marked.min.js) (via CDN)
- **Fonts**: Google Fonts (`Fraunces`, `Inter`, `IBM Plex Mono`)

---

## 📁 Repository Structure

```
.
├── md_file_viewer.html      # Complete standalone web application
├── level2_game_story.md     # Optional default sample file
└── README.md                # Documentation
```

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
