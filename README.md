# LandingPage

A minimal **draggable dashboard** landing page built with Bootstrap.
Users can rearrange cards representing application sections, save the order to `localStorage`, and export/import or reset that order. This repo is intended as a simple starting point or demo for creating customizable dashboard layouts.

---

## 🚀 Features

- Responsive grid of cards using Bootstrap 5
- Drag & drop reordering with visual cues and a little "jiggle" during drag
- Persist order in `localStorage` so the layout survives page reloads
- Export order to JSON file
- Upload a previously exported JSON to restore a layout
- Reset to default arrangement
- Customizable footer color via CSS variable
- Clickable cards navigate to the associated URL (placeholder links by default)

> The logic lives entirely in the single `index.html` file; there are no build steps or dependencies.

---

## 🛠️ Usage

1. Clone or download the repository.
2. Open `index.html` in a modern browser (Chrome, Firefox, Edge, Safari).
3. Drag cards around to change their order. The new order will be saved automatically.
4. Use the buttons in the footer to export, upload, or reset the card order.

#### Customization

- Edit the `defaultCards` array in `index.html` to change titles, images, target URLs, and descriptions.
- Override the `--footer-bg-color` variable in `:root` to match your branding.
- Replace the placeholder navigation links with real routes.

---

## 💾 Persistence

The card order is stored under the `cardOrder` key in `localStorage` as a JSON array of card IDs. You can manually clear it via browser dev tools or use the **Reset order** button.

---

## 📄 License

This project is provided under the [MIT License](LICENSE) (if you choose to add one). Feel free to adapt it for personal or commercial use.

---

## 📎 Acknowledgements

Built using [Bootstrap](https://getbootstrap.com) and inspired by simple dashboard layouts. The drag & drop behavior uses native HTML5 APIs with minimal custom JavaScript.

Enjoy! 🎉
