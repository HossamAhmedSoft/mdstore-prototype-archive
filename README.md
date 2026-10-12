# MD Boutique — E-Commerce Progressive Web App (PWA) Prototype

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-F7DF1E?logo=javascript&logoColor=black)
![PWA](https://img.shields.io/badge/PWA-Service%20Worker%20%7C%20Manifest-5A0FC8?logo=pwa&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

A multi-page e-commerce **Progressive Web Application (PWA)** prototype for a luxury cosmetics and skincare boutique. Built purely with semantic HTML5, modern vanilla CSS3, and vanilla JavaScript with offline asset caching and shopping cart state management.

---

## Features & Architectural Highlights

- **Progressive Web App Architecture:** Configured with `manifest.json` for standalone app installation and `sw.js` (Service Worker) for asset pre-caching and offline capability.
- **Client-Side Cart & Store Management:** `js/store.js` and `js/app.js` handle reactive product filtering, quantity calculation, local storage persistence, and checkout totals.
- **Multi-Page Shopping Experience:**
  - `index.html`: Boutique storefront with promotional hero sliders and category cards.
  - `collections/*.html`: Segmented product catalogs for Skincare and Makeup collections.
  - `product.html`: Detailed single-product view with gallery thumbnails and add-to-cart controls.
  - `cart.html` & `checkout.html`: Shopping cart drawer and multi-step order placement flow.
  - `order-confirmation.html`: Order summary and simulated transaction completion.
  - `Pages/*.html`: Ancillary views including About Us, Contact, Order Tracking, and Account Login.
- **Zero Third-Party Runtime Dependencies:** 100% vanilla web stack without heavy frameworks.

---

## Project Structure

```
mdstore-prototype-archive/
├── index.html                 # Main boutique storefront
├── cart.html                  # Cart management page
├── checkout.html              # Multi-step checkout
├── product.html               # Product detail view
├── order-confirmation.html    # Confirmation receipt view
├── manifest.json              # Web app manifest
├── sw.js                      # Service Worker offline caching logic
├── collections/               # Category catalog templates
├── Pages/                     # Secondary user pages (about, contact, login, tracking)
├── css/                       # Boutique stylesheet (sofie.css)
├── js/                        # Application, store, and UI controllers
└── img/                       # Product photography and banners
```

---

## Running Locally

Because Service Workers require a secure origin (`http://localhost` or HTTPS), serve the directory via any local web server:

```bash
# Using Python
python -m http.server 8080

# Using Node.js
npx serve .
```

Open `http://localhost:8080` in any modern web browser.

---

## Author & License

- **Developer:** Hossam Ahmed ([@HossamAhmedSoft](https://github.com/HossamAhmedSoft))
- **License:** MIT
