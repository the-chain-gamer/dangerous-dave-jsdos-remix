# Credits

This project brings **Dangerous Dave (1990, MS-DOS)** to the web using **js-dos v8** and a lightweight HTML wrapper with on-screen controls and Remix (Farcade) integration.

---

## Game

- **Title:** Dangerous Dave (DOS)
- **Year:** 1990
- **Original creators:** **John Romero** / **Softdisk**
- **Rights:** © Softdisk / John Romero.  
- **Distribution:** Commonly distributed as **freeware**; this project embeds the **unmodified** game data solely for non-commercial access and preservation. See `NOTICE` for details.

If you are a rights holder and want this removed, please contact **thechaingamer1@gmail.com**.

---

## Emulator / Player

- **js-dos v8** — DOSBox in WebAssembly  
  - Author: **@caiiiycuk** & contributors  
  - License: **GPL-2.0**  
  - Site/Docs: https://js-dos.com/  
  - Source: https://github.com/caiiiycuk/js-dos
- **DOSBox** (upstream core)  
  - The DOS emulator powering js-dos  
  - License: **GPL-2.0**  
  - Site: https://www.dosbox.com/

---

## Web Wrapper & Controls

- **Author:** **Ali (@the-chain-gamer)**
- **What:** HTML launcher, always-visible touch controls (◀ ▼ ▶ with ▲ above), auto-boot into `DDAVE\DAVE.EXE`, and landscape rotation shell for Remix.
- **License:** **MIT** (see `LICENSE`).  
  *(This license covers only the wrapper code and not the original game data.)*

---

## Remix / Farcade Integration

- **SDK:** `@farcade/game-sdk`
- **What:** Signals `ready()`, handles `play_again` / `toggle_mute`, and triggers haptic feedback on key actions (CTRL/ALT).
- **Attribution:** © Farcade / Remix.  
- **CDN:** `https://cdn.jsdelivr.net/npm/@farcade/game-sdk@latest/dist/index.min.js`

---

## Hosting

- **GitHub Pages** — static hosting for the player + bundle.
- The Remix mini-app loads this page in an `<iframe>` and provides the portrait container; the page handles rotation/scaling.

---

## Third-Party Assets & CDNs

- **js-dos v8 CDN:** `https://v8.js-dos.com/latest/`  
  Files used: `js-dos.js`, `js-dos.css` (and optional `wdosbox.*` if self-hosted)
- **(Optional) Self-hosted runtime:** `js-dos/` with `emulators/wdosbox.{js,data,wasm,worker.js}`

---

## NOTICE (summary)

- *Dangerous Dave (1990) © Softdisk / John Romero — redistributed for free, unmodified.*  
- The Gamer’s Edge sampler disk containing Dangerous Dave is free to distribute **if its contents are unaltered**.  
- This project embeds the game only for **non-commercial** access and preservation.  
- **js-dos v8** and **DOSBox** are GPL-licensed projects; the wrapper code here is MIT-licensed.

See `NOTICE` and `README.md` for licensing details.

---

## Acknowledgements

- John Romero & the Softdisk team — for the game.
- @caiiiycuk & js-dos contributors — for making DOS games run beautifully on the web.
- The DOSBox team — for the emulator core.
- Remix / Farcade — for the mini-app platform and SDK.
