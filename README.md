# **📚 Complete MuPDF Guide for Linux (Ubuntu, Fedora, Arch) 🐧**

MuPDF is the **lightning-fast ⚡** PDF viewer that works across all major Linux distros! 
Here's how to install and use it everywhere:

## **🛠 Installation on Different Distros**

### **Ubuntu/Debian 🐳**
```bash
sudo apt update
sudo apt install mupdf mupdf-tools  # Includes CLI utilities
```

### **Fedora/RHEL 🎩**
```bash
sudo dnf install mupdf mupdf-tools
```

### **Arch Linux/Manjaro 🏗️**
```bash
sudo pacman -S mupdf mupdf-tools
```

### **OpenSUSE 🦎**
```bash
sudo zypper install mupdf mupdf-tools
```

## **🏁 Basic Usage (All Distros)**
```bash
mupdf document.pdf          # GUI mode
mupdf -T document.pdf       # Terminal mode (no X11 needed)
```

## **🎮 Universal Keyboard Controls**
| Key | Action | Emoji |
|-----|--------|-------|
| Arrows | Navigate | 🧭 |
| PgUp/PgDn | Change page | 📄 |
| +/- | Zoom | 🔍 |
| 0 | Reset zoom | 🔄 |
| / | Search | 🔎 |
| f | Fullscreen | 🖥️ |
| q | Quit | 🚪 |

## **⚡ Advanced Features (Works Everywhere)**
```bash
# Extract text
mutool draw -F txt input.pdf > output.txt

# Extract images
mutool extract input.pdf

# Merge PDFs
mutool merge file1.pdf file2.pdf merged.pdf

# Presentation mode
mupdf -P slides.pdf
```

## **⚙️ Configuration**
Create config file at `~/.config/mupdf/settings`:
```ini
# Works on all distros
antialias=10    # Smoother text (1-10)
background=eeeeee  # Light gray bg
fontsize=12
```

## **🚀 Performance Tips**
```bash
mupdf -r 72 bigfile.pdf    # Faster rendering
mupdf -A0 crisp.pdf       # Disable anti-aliasing
```

## **MuPDF the best**
✅ **Same great experience on all distros**  
✅ **Lightest PDF viewer available** (uses just ~10MB RAM!)  
✅ **Terminal-friendly** for servers/SSH work  
✅ **Includes powerful `mutool` CLI**  
