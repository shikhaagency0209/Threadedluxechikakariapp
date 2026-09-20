[README.md](https://github.com/user-attachments/files/32441008/README.md)
# Threaded Luxe Chikankari Design Studio

**You Choose. We Embroider.**

A single-file, browser-based design customizer for Threaded Luxe Chikankari. Customers pick a garment, recolour it, hand-place Chikankari embroidery motifs, choose a size, and check out — no build step, no server, no dependencies beyond what loads from CDN.

## ✨ Features

- **Garment picker** — shirts, dresses, tops, tunics, one-piece, and co-ord sets, with sample garments preloaded
- **Live colour customization** — recolour any garment while preserving its fabric texture, folds, and shading
- **Chikankari embroidery library** — lotus, rose, paisley, leaves, buti, bel, jaal, and more, with drag, resize, rotate, duplicate, and delete on canvas
- **Thread colour & fabric picker** — Mulmul, Cotton, Rayon, Modal, Georgette, Chanderi, and more
- **Custom uploads** — customers/admins can upload their own garment photos and embroidery motifs directly in the browser
- **My Designs gallery** — save, revisit, and re-order past designs
- **Size selection & automatic price calculator** — base garment price + ₹200 per placed motif, computed live
- **Checkout flow** — order details are handed to the customer's email app (pre-filled to your inbox) and to WhatsApp for payment confirmation
- **Local admin panel** — email/password-gated view of orders, customer details, sizes, payment status, and shipping/tracking, editable in place
- **Backup & restore** — export uploaded garments, motifs, and saved designs to a JSON file, and re-import them anywhere
- **Mobile-friendly, premium UI** — built for phones first, since most customers will land here from Instagram

## 🧵 Tech

Plain HTML, CSS, and vanilla JavaScript, rendered on an HTML5 canvas. No React/build tooling — the whole app is one `.html` file so it can be opened directly, hosted on any static file host, or embedded. Persistence (uploads, saved designs, orders) uses the browser's `localStorage`.

## 🚀 Running it

No build step required.

- **Locally:** download `threaded-luxe-studio.html` and open it in any modern browser.
- **Hosted:** drop the file into any static host (GitHub Pages, Netlify, Vercel) — rename it to `index.html` for the cleanest URL.

### GitHub Pages
1. Push this repo, with the file renamed to `index.html` at the root (or in `/docs`).
2. Repo **Settings → Pages** → set the source branch/folder.
3. Your live link is `https://<username>.github.io/<repo>/`.

## ⚠️ Known limitations

This is a front-end-only app — there is no backend or database:

- **Orders and the admin panel are per-browser.** An order reaches you reliably by email and WhatsApp regardless of the customer's device, but the admin dashboard only shows orders placed *on the device it's opened on*. A shared, multi-device order log needs a real backend.
- **The admin login is a local gate, not real security.** It's stored (lightly obfuscated, not encrypted) in the browser's storage, meant to keep the order list private on your own device — not to secure a public storefront.
- **Uploads live in browser storage too.** Use the built-in **Backup my uploads / Restore** buttons to move garments, motifs, and designs between browsers or devices, or to guard against a browser storage reset.

## 📄 License

Add your preferred license here (e.g., MIT, or "All rights reserved" if this is proprietary to Threaded Luxe Chikankari).
