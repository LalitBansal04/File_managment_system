# 📂 Automated Downloads Folder Organizer (Python)

A **real-time file organization automation tool** built with Python that monitors your **Downloads folder** and automatically sorts files into appropriate system folders such as **Documents, Images, Videos, Music, and Sound Effects** based on file extensions and size.

This project uses the **Watchdog** library to observe filesystem changes and perform actions instantly when new files are created.

---

## 🚀 Features

* 🔍 **Real-time monitoring** of the Downloads folder
* 📁 Automatically organizes files by type:

  * 📄 Documents → Documents folder
  * 🖼️ Images → Pictures folder
  * 🎥 Videos → Videos folder
  * 🎵 Audio → Music / SFX folder
* 🎧 Smart audio handling:

  * Small audio files or files containing `SFX` go to the SFX folder
  * Large audio files go to the Music folder
* 🔁 **Duplicate file handling** (auto-renames files)
* 🧾 **Logging** for tracking moved files
* ⚙️ Fully automated background process

---

## 🛠️ Technologies Used

* **Python 3**
* **watchdog** (filesystem monitoring)
* **os / shutil** (file operations)
* **logging** (activity tracking)

---

## 📁 Folder Structure

```text
Downloads/
├── song.mp3        → Music/
├── image.png       → Pictures/
├── video.mp4       → Videos/
├── report.pdf      → Documents/
├── click_sfx.wav   → Music (SFX)
```

---

## 📦 Supported File Types

### Images

`.jpg .jpeg .png .gif .bmp .svg .webp .tiff .heic`

### Videos

`.mp4 .mkv .avi .mov .wmv .flv`

### Audio

`.mp3 .wav .aac .flac .m4a`

### Documents

`.pdf .docx .doc .pptx .xlsx .txt`

---

## 🔧 Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/automated-downloads-organizer.git
cd automated-downloads-organizer
```

### 2️⃣ Install dependencies

```bash
pip install watchdog
```

### 3️⃣ Configure paths

Edit the directory paths in the script if needed:

```python
source_dir = "C:\\Users\\UserName\\Downloads"
```

---

## ▶️ Usage

Run the script:

```bash
python main.py
```

The script will:

* Start running in the background
* Automatically move files as soon as they appear in the Downloads folder

To stop the script:

```bash
CTRL + C
```

---

## 📝 Logging

All file movements are logged with timestamps:

```text
2025-01-01 12:30:45 - Moved audio file: song.mp3
```

---

## 📌 Future Enhancements

* 🪟 Run automatically on Windows startup
* 🖥️ GUI using Tkinter or PyQt
* ⚙️ Configuration via JSON/YAML
* 🧪 Unit tests
* 📦 Convert to executable (.exe)

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 👨‍💻 Author

**Your Name**
📧 Email: [your-email@example.com](bansal.lalit2004@gmail.com)
🔗 GitHub: [https://github.com/your-username](https://github.com/LalitBansal04)

---

⭐ If you found this project useful, consider giving it a star!
