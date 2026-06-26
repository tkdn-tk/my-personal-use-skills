---
name: ascii-art
description: Generate and search for ASCII art, including text banners (pyfiglet/asciified), message art (cowsay), decorative borders (boxes), colored text (TOIlet), and image-to-ASCII conversion. Use when the user mentions ASCII art, text banners, cowsay, or wants to stylize text/images into characters.
---

# ASCII Art Skill
Multiple tools for different ASCII art needs. All tools are local CLI programs or free REST APIs — no API keys required.

## Tool 1: Text Banners (pyfiglet — local)
Render text as large ASCII art banners. 571 built-in fonts.

### Setup
`pip install pyfiglet --break-system-packages -q`

### Usage
- `python3 -m pyfiglet "YOUR TEXT" -f slant`
- `python3 -m pyfiglet "TEXT" -f doom -w 80` # Set width
- `python3 -m pyfiglet --list_fonts` # List all 571 fonts

### Recommended fonts
- **slant**: Clean & modern (Project names, headers)
- **doom**: Bold & blocky (Titles, logos)
- **big**: Big & readable (Banners)
- **banner3**: Classic banner (Wide displays)
- **small**: Compact (Subtitles)
- **cyberlarge**: Cyberpunk (Tech themes)
- **3-d**: 3D effect (Splash screens)
- **gothic**: Gothic (Dramatic text)

---

## Tool 2: Text Banners (asciified API — remote, no install)
Free REST API that converts text to ASCII art. 250+ FIGlet fonts. Returns plain text directly.

### Usage (via terminal curl)
- `curl -s "https://asciified.thelicato.io/api/v2/ascii?text=Hello+World"`
- `curl -s "https://asciified.thelicato.io/api/v2/ascii?text=Hello&font=Slant"`
- `curl -s "https://asciified.thelicato.io/api/v2/fonts"` # List all fonts

---

## Tool 3: Cowsay (Message Art)
Classic tool that wraps text in a speech bubble with an ASCII character.

### Setup
- `sudo apt install cowsay -y` # Debian/Ubuntu
- `brew install cowsay` # macOS

### Usage
- `cowsay "Hello World"`
- `cowsay -f tux "Linux rules"` # Tux the penguin
- `cowsay -f dragon "Rawr!"` # Dragon
- `cowsay -l` # List all characters

---

## Tool 4: Boxes (Decorative Borders)
Draw decorative ASCII art borders/frames around any text. 70+ built-in designs.

### Setup
- `sudo apt install boxes -y` # Debian/Ubuntu
- `brew install boxes` # macOS

### Usage
- `echo "Hello World" | boxes`
- `echo "Hello World" | boxes -d stone` # Stone border
- `echo "Hello World" | boxes -d parchment` # Parchment scroll
- `echo "Hello World" | boxes -d cat` # Cat border

---

## Tool 5: TOIlet (Colored Text Art)
Like pyfiglet but with ANSI color effects and visual filters.

### Setup
- `sudo apt install toilet toilet-fonts -y` # Debian/Ubuntu
- `brew install toilet` # macOS

### Usage
- `toilet --gay "Rainbow!"` # Rainbow coloring
- `toilet --metal "Metal!"` # Metallic effect
- `toilet -F border "Bordered"` # Add border

---

## Tool 6: Image to ASCII Art
Convert images (PNG, JPEG, GIF, WEBP) to ASCII art.

### Option A: ascii-image-converter (recommended)
- `sudo snap install ascii-image-converter`
- `ascii-image-converter image.png -C` # Color output

### Option B: jp2a (lightweight, JPEG only)
- `sudo apt install jp2a -y`
- `jp2a --width=80 image.jpg`

---

## Tool 7: Search Pre-Made ASCII Art
Search curated ASCII art from the web.

### Source A: ascii.co.uk
URL pattern: `https://ascii.co.uk/art/{subject}`
Subjects include: `cat`, `dog`, `car`, `rocket`, `tree`, `skull`, `robot`, etc.

### Source B: GitHub Octocat API
`curl -s https://api.github.com/octocat`

---

## Tool 8: Fun ASCII Utilities (via curl)
- **QR Codes**: `curl -s "qrenco.de/Hello+World"`
- **Weather**: `curl -s "wttr.in/London"`
- **Moon Phase**: `curl -s "wttr.in/Moon"`

---

## Tool 9: LLM-Generated Custom Art (Fallback)
Generate ASCII art directly using Unicode characters (Box Drawing, Block Elements, Geometric Symbols).

### Decision Flow
1. **Text Banner**: `pyfiglet` or `asciified API`.
2. **Message Bubble**: `cowsay`.
3. **Border/Frame**: `boxes`.
4. **Specific Object**: `ascii.co.uk`.
5. **Image Conversion**: `ascii-image-converter`.
6. **QR/Weather**: `qrenco.de` or `wttr.in`.
7. **Custom**: LLM generation.
