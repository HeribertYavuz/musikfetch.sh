# musikfetch 🎵

**musikfetch** is a simple and stable Bash script that displays information about the currently playing music (title, artist, album) and, when possible, shows the **album cover directly in the terminal**. It is designed especially for *minimal* and *rice*-focused Linux setups.
<img width="1920" height="1080" alt="20251213_19h57m23s_grim" src="https://github.com/user-attachments/assets/f0164954-3aaa-46e6-85e8-4a1e3d90ec3b" />

---

## ✨ Features

* 🎶 Displays currently playing track information (MPRIS-compatible players)
* 🖼️ Terminal album cover support (Kitty / WezTerm)
* 🧱 ASCII placeholder for unsupported terminals
* 🎨 Clean, readable, colored output
* ⚡ Lightweight, fast, standalone Bash script

---

## 📦 Requirements

The following tools must be installed on your system:

* `bash`
* `playerctl`
* `curl`
* `jq`

For album cover display:

* **Kitty** or **WezTerm** terminal emulator

> The script works with MPRIS-compatible music players such as Spotify, VLC, mpd, etc.

---

## 🛠️ Installation

```bash
git clone https://github.com/yourusername/musikfetch.git
cd musikfetch
chmod +x musikfetch.sh
```

Optional: install globally

```bash
sudo cp musikfetch.sh /usr/local/bin/musikfetch
```

---

## ▶️ Usage

```bash
./musikfetch.sh
```

If installed globally:

```bash
musikfetch
```

---

## 🔗 Alias Usage

If you prefer not to install the script globally, you can create an alias so that typing **`musikfetch`** runs the script in the background.

### Bash / Zsh

```bash
alias musikfetch='bash /path/to/musikfetch.sh'
```

To make it permanent, add the line above to one of the following files:

* `~/.bashrc`
* `~/.zshrc`

Then reload your shell configuration:

```bash
source ~/.bashrc   # or source ~/.zshrc
```

Now you can simply run:

```bash
musikfetch
```

---

## 🖥️ Terminal Behavior

* **Kitty / WezTerm**

  * Album cover is rendered directly inside the terminal

* **Other terminals**

  * An ASCII placeholder is shown instead
  * Track information is still displayed normally

---

## 📸 Example Output

```
♪ Now Playing
────────────
Title  : Everlong
Artist : Foo Fighters
Album  : The Colour and the Shape
```

(Album art appears above when using Kitty or WezTerm)

---

## ⚠️ Notes

* If no music is playing, output may be empty
* When multiple players are active, `playerctl` selects the default one
* Works on both Wayland and X11 environments

---

## 📄 License

MIT License

---

## 💚 Contributing

Issues, suggestions, and pull requests are always welcome!

> *"Even small tools can make a big difference when used in the right place."* ✨
