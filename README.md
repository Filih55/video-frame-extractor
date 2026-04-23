# 🎬 Video Frame Extractor – Ultimate Edition

Extract high-quality frames from any video file with automatic rotation detection, multi-engine processing, and one-click ZIP download. Perfect for video analysis, thumbnailing, or frame-by-frame inspection.

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=flat&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=flat&logo=javascript&logoColor=%23F7DF1E)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=flat&logo=tailwind-css&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green)

---

## ✨ Features

- 🎥 **Supports all major video formats** (MP4, MOV, AVI, MKV, etc. via browser capabilities)
- 🔄 **Automatic rotation detection** – reads metadata from MP4/MOV to correctly orient portrait videos
- ⚙️ **Three processing engines**:
  - **Ultimate** – best quality & rotation accuracy (balanced speed)
  - **Accurate** – precise frame seeking using `requestVideoFrameCallback`
  - **Fast** – quicker extraction, suitable for previews
- 🎛️ **Flexible extraction controls**:
  - Start / end frame selection
  - Custom frame interval (extract every Nth frame)
  - Output format: JPEG (adjustable quality) or PNG (lossless)
  - Manual rotation override (0°/90°/180°/270°)
- 🖼️ **Live gallery preview** – extracted frames appear instantly with thumbnails
- 💾 **Batch download** – all frames as a single ZIP file
- ⌨️ **Keyboard shortcuts** – play/pause, next/previous frame, escape to close lightbox
- 🪄 **Modern dark UI** – fully responsive, glass-morphism design

---

## 🚀 Demo / Usage

You Can TRY HERE : https://learningprojectin.blogspot.com/2026/04/videoframes-capture.html

1. **Open the tool** in any modern browser (Chrome, Edge, Firefox, Safari).
2. **Upload a video** via drag & drop or file picker.
3. The tool automatically detects video dimensions, FPS, and rotation.
4. Adjust extraction parameters (frame range, interval, format, quality, rotation override).
5. Click **Start Extraction** – frames will be captured and displayed in the gallery.
6. **Download** individual frames or the entire set as a ZIP file.

> 💡 **Pro tip**: Use the keyboard arrow keys to step through frames before extraction to find the perfect range.

---

## 🧠 How It Works

- The video is loaded into an HTML5 `<video>` element.
- Frame extraction is done by drawing the current video frame onto a hidden `<canvas>`.
- Rotation is applied either automatically (from metadata) or manually via canvas transformation.
- The `requestVideoFrameCallback` API ensures frame-accurate seeking (fallback to `seeked` event).
- Extracted frames are stored as Blobs and displayed using object URLs.
- JSZip + FileSaver.js are used to package frames into a ZIP archive.

---

## 🛠️ Tech Stack

- **HTML5 / CSS3** – semantic markup, Tailwind CSS for styling
- **JavaScript (ES6+)** – core logic, async processing, DOM manipulation
- **Canvas API** – frame rendering and rotation
- **File API** – video file handling and Blob management
- **JSZip** – ZIP archive creation
- **FileSaver.js** – client-side file download

---

## 📂 Project Structure

> The entire tool is self-contained in one HTML file – no build step required.

---

## 🔧 Installation & Local Run

No dependencies or server needed. Just clone and open:

```bash
git clone https://github.com/FILIH55/video-frame-extractor.git
cd video-frame-extractor
open index.html

Or use a local dev server (e.g., npx serve .)

🧪 Browser Compatibility
Works on all modern browsers that support:

HTML5 <video> and <canvas>

requestVideoFrameCallback (fallback provided)

File API and Blob

ES6 Promises

Tested on: Chrome 120+, Firefox 121+, Safari 17+, Edge 120+.

🤝 Contributing
Contributions are welcome! If you have ideas for:

New engines (e.g., WebCodecs for performance)

Multi-threaded extraction

Video trimming integration

More metadata extraction (e.g., GPS from MOV)

Please open an issue or submit a pull request.

📄 License
MIT License – free for personal and commercial use.

🙏 Acknowledgements
Tailwind CSS for the utility-first CSS framework

JSZip and FileSaver.js

Google Material Symbols for icons

Made with ⚡ and ❤️ for video creators, analysts, and developers.
