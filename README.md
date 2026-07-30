# POW! Password Generator 💥

A single-page, comic-book-themed password generator built with plain **HTML, CSS, and JavaScript** — no frameworks, no build step, no dependencies. Just open the file in a browser.

![Theme](https://img.shields.io/badge/theme-comic-yellow) ![No Dependencies](https://img.shields.io/badge/dependencies-none-brightgreen)

## Features

- 🎨 **Comic-book UI** — bold outlines, halftone dots, speech-bubble output box, Bangers/Comic Neue fonts
- 🌗 **Light / Dark mode toggle** — flips the whole palette between a bright comic-panel look and a comic-noir dark mode
- 🎚️ **Adjustable length slider** (4–32 characters) — updates the generated password live as you drag
- ✅ **Configurable character sets** — toggle numbers, special characters, and uppercase letters on/off
- 🛡️ **Guaranteed character coverage** — if you enable numbers/specials/uppercase, the generator guarantees at least one of each appears (and shuffles the result so they're not clustered at the end)
- 📋 **One-click copy** to clipboard with a comic-style "COPIED!" toast
- 💪 **Strength badge** based on password length:
  | Length | Label | Color |
  |---|---|---|
  | ≤ 7 | WEAK | Red |
  | 8–10 | Acceptable | Yellow |
  | 11–14 | Strong | Purple |
  | 15+ | Boom! | Cyan |

## Getting Started

No installation needed.

1. Clone or download this repo
2. Open `password-generator.html` in any modern browser (Chrome, Firefox, Edge, Safari)

```bash
git clone <your-repo-url>
cd <your-repo-folder>
open password-generator.html   # or just double-click the file
```

## Usage

1. Drag the **LENGTH** slider to set how long you want the password (4–32 characters)
2. Toggle the checkboxes for **Numbers**, **Special Characters**, and **Uppercase Letters**
3. Click **GENERATE!** to create a new password
4. Click **COPY!** to copy it to your clipboard
5. Use the switch in the top-right corner to toggle **Light / Dark** mode

## Project Structure

```
.
├── password-generator.html   # Everything — markup, styles, and logic in one file
├── Password_Generator.py     # Original Python CLI version this project is based on
└── README.md
```

## Background

This started as a simple Python CLI script (`Password_Generator.py`) that asked for a minimum length and whether to include numbers/special characters. This web version reimplements and improves on that logic:

- Fixes a bug in the original where the "meets criteria" check didn't correctly validate all selected character types together
- Removes a stray leading space that was present in every generated password
- Adds a browser-based UI with live controls instead of terminal prompts

## Tech Stack

- HTML5
- CSS3 (custom properties / CSS variables for theming, no framework)
- Vanilla JavaScript (no libraries)
- [Google Fonts](https://fonts.google.com/) — Bangers & Comic Neue

## License

Feel free to use, modify, and share this project. Add a license file (MIT, for example) if you plan to publish it publicly.

## Contributing

This is a personal portfolio project, but suggestions and pull requests are welcome — feel free to open an issue if you spot a bug or have an idea for a new comic theme variant.
