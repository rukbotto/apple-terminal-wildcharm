# Wildcharm Apple Terminal Profile

Wildcharm is an Apple Terminal profile with a curated ANSI palette and dynamic colors that adapt to light and dark system themes, inspired by the Wildcharm color scheme for the VIM editor.

## Download
Download the profile file to your computer using one of these options:
- From the repository UI, click `Wildcharm.terminal` and choose “Download”.
- From a terminal, run:
    ```sh
    curl -L -o Wildcharm.terminal https://raw.githubusercontent.com/rukbotto/apple-terminal-wildcharm/master/Wildcharm.terminal
    ```
- To download the pastel variant:
    ```sh
    curl -L -o Wildcharm-Pastel.terminal https://raw.githubusercontent.com/rukbotto/apple-terminal-wildcharm/master/Wildcharm-Pastel.terminal
    ```
- To download the dark variants:
    ```sh
    curl -L -o Wildcharm-Dark.terminal https://raw.githubusercontent.com/rukbotto/apple-terminal-wildcharm/master/Wildcharm-Dark.terminal
    curl -L -o Wildcharm-Pastel-Dark.terminal https://raw.githubusercontent.com/rukbotto/apple-terminal-wildcharm/master/Wildcharm-Pastel-Dark.terminal
    ```
- Or clone the repo and use the file locally:
    ```sh
    git clone https://github.com/rukbotto/apple-terminal-wildcharm.git
    cd apple-terminal-wildcharm
    ```

## Install
- Double-click a `.terminal` file to import (for example `Wildcharm.terminal`, `Wildcharm-Pastel.terminal`, or `Wildcharm-Dark.terminal`), or run:

```sh
open Wildcharm.terminal
```

Then set it as default in Terminal → Settings → Profiles → the imported profile → Default.

## Features
- ANSI palette tuned to the provided 16‑color scheme, with Pastel, Dark, and Pastel Dark variants.
- Background and text colors follow the system light/dark appearance.
- Cursor uses dynamic text color for contrast on both themes.
- Dark variants use a standalone black background with a light foreground and the existing ANSI palette.

## Samples
- `wildcharm-sample.html`: HTML preview of the Wildcharm palette.
- `wildcharm-pastel-sample.html`: HTML preview of the Wildcharm Pastel palette.
- `wildcharm-dark-sample.html`: HTML preview of the Wildcharm Dark palette.
- `wildcharm-pastel-dark-sample.html`: HTML preview of the Wildcharm Pastel Dark palette.

## Notes
If colors look incorrect after import, remove and re‑import the profile, then ensure Terminal is using the “Wildcharm” profile for the current window.
