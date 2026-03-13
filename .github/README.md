# LandingPage

A minimal **draggable dashboard** landing page built with Bootstrap.
Users can rearrange cards representing application sections, save the order to `localStorage`, and export/import or reset that order. This repository serves both as a simple demo of a customizable layout and as a starting point for an **internal company dashboard** where employees can personalize their workspace.

---

## 🚀 Core Features

- Responsive grid of cards using Bootstrap 5.
- Drag & drop reordering with visual cues during drag.
- Persist order in `localStorage` so the layout survives page reloads.
- Export order to a JSON file (hover over the button for a quick tip).
- Upload a previously exported JSON to restore a layout.
- Reset to default arrangement.
- 🎨 Customizable background color via CSS variable.
- Clickable cards navigate to the associated URL (placeholder links by default).

> All logic lives entirely in the single `index.html` file; no build steps or external dependencies are required.

---

## 🛠️ Usage

1. Clone or download the repository.
2. Open `index.html` in a modern browser (Chrome, Firefox, Edge, Safari).
3. Drag cards around to change their order. The new order will be saved automatically.
4. Use the buttons in the footer to export, upload, or reset the card order.

### Customization

- Edit `config.json` to change branding (site name, links, footer text), card definitions, and theme colors. Everything on the page can be configured via this file; no manual CSS edits are needed.
- Modify the `defaultCards` array in `index.html` only if you need a quick prototype without the config file.
- Replace placeholder navigation links with real routes, either in `config.json` or directly in the HTML.

---

## 💾 Persistence

The card order is stored under the `cardOrder` key in `localStorage` as a JSON array of card IDs. Clear it via browser dev tools or use the **Reset order** button.

---

## 📄 License

This project is provided under the [Creator's License](./LICENSE.md). **Please read the license file carefully before using or distributing the code. It is **

---

## 📎 Acknowledgements

Built using [Bootstrap](https://getbootstrap.com) and inspired by simple dashboard layouts. The drag & drop interactions use native HTML5 APIs with minimal custom JavaScript.

Thanks to **Raptor mini** for documentation assistance. 🛠️

Enjoy! 🎉
