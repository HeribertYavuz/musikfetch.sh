musikfetch 🎵

A beautiful CLI tool that displays currently playing music information with album art in your terminal.
Features ✨

    🎨 Album Art Display: Shows album cover in Kitty terminal

    🖼️ ASCII Fallback: Displays ASCII art in other terminals

    🎵 Music Info: Shows title, artist, album, and playback status

    ⏱️ Progress Bar: Visual progress indicator with time display

    🚀 Lightweight: Fast and minimal - no bloat

    🎯 Simple: One command, instant results

Preview 📸
text

▓▒░ musikfetch v1.0.0 ░▒▓

ALBUM ART
[Album cover displayed here in Kitty]

NOW PLAYING
──────────────────────────────
▶ Playing
🎵 Title:  Bohemian Rhapsody
🎤 Artist: Queen
💿 Album:  A Night at the Opera
⏱  Progress: 02:15 / 05:55
[███████████───────────] 38%
──────────────────────────────

Installation 📦
Quick Install
bash

# Download and install
curl -sL https://raw.githubusercontent.com/YOUR_USERNAME/musikfetch/main/musikfetch -o musikfetch
chmod +x musikfetch
sudo mv musikfetch /usr/local/bin/

Manual Install
bash

# Clone repository
git clone https://github.com/YOUR_USERNAME/musikfetch.git
cd musikfetch

# Make executable
chmod +x musikfetch

# Install globally (optional)
sudo cp musikfetch /usr/local/bin/

Dependencies ⚙️
Required:

    playerctl - For music player control
    bash

# Ubuntu/Debian
sudo apt install playerctl

# Arch
sudo pacman -S playerctl

# Fedora
sudo dnf install playerctl

Optional but Recommended:

    Kitty Terminal - For actual album art display

        Install: kitty terminal

Usage 🚀

Simply run:
bash

musikfetch

Options:
bash

musikfetch --help      # Show help message
musikfetch --version   # Show version info
musikfetch --no-clear  # Don't clear screen before display

Supported Players 🎧

Any MPRIS-compatible media player:

    Spotify

    VLC

    Rhythmbox

    Firefox (when playing media)

    Chromium/Chrome (when playing media)

    And many more...

Terminal Support 🖥️
Terminal	Album Art	ASCII Fallback
Kitty	✅ Full color image	-
Other terminals	❌	✅ ASCII art
Examples 📝
bash

# Basic usage
musikfetch

# Keep terminal history (don't clear)
musikfetch --no-clear

# Check version
musikfetch --version

# Quick check with curl
curl -sL https://raw.githubusercontent.com/YOUR_USERNAME/musikfetch/main/musikfetch | bash -s --

How It Works 🔧

    Fetches metadata from your music player using playerctl

    Retrieves album art URL from player metadata

    Displays image in Kitty using kitten icat

    Shows ASCII art in other terminals

    Formats output with colors and progress bar

Troubleshooting 🔍
"No active music player detected"

    Make sure a media player is running

    Check if your player supports MPRIS

"playerctl is not installed"

    Install playerctl using package manager

    See Dependencies section

Album art not showing in Kitty

    Ensure you're using Kitty terminal

    Try updating Kitty to latest version

Contributing 🤝

Contributions are welcome! Here's how:

    Fork the repository

    Create a feature branch (git checkout -b feature/AmazingFeature)

    Commit your changes (git commit -m 'Add AmazingFeature')

    Push to the branch (git push origin feature/AmazingFeature)

    Open a Pull Request

Development
bash

# Test changes locally
./musikfetch

# Debug mode
bash -x musikfetch

Roadmap 🗺️

    Configuration file support

    Multiple output formats

    More ASCII art styles

    Integration with music APIs

    Themes and color schemes

License 📄

This project is licensed under the MIT License - see the LICENSE file for details.
Acknowledgments 🙏

    Inspired by FastFetch and similar CLI tools

    Uses playerctl for music player interaction

    Thanks to Kitty terminal developers for awesome image support

    All the amazing open-source projects that made this possible

Support 💬

Found a bug? Have a feature request?

    Open an Issue

    Star the repository if you like it! ⭐

Made with ❤️ for music lovers and terminal enthusiasts

"Music is the soundtrack of your life." 🎶
