# Kanpur Sweet House Landing Page Template

A premium, responsive, and high-converting single-page website template designed for traditional local Sweet Houses (Mithai & Snacks shops) in Kanpur, India. 

This repository serves as a visual sales demo and ready-to-use template for local business owners looking to digitize their storefront, offer festival pre-orders, and accept orders directly via WhatsApp.

---

## ✨ Features

- **Royal Indian Heritage Theme**: Designed with a curated palette of Deep Crimson/Maroon (`#800020`), Rich Ochre/Gold (`#D4AF37`), and clean Cream backgrounds (`#FDFBF7`).
- **Premium Typography**: Serif headings (Playfair Display) paired with modern, readable body text (Inter).
- **Responsive Layout**: Designed with mobile-first principles to look flawless on smartphones, tablets, and desktop displays.
- **WhatsApp Order Integration**: Features a dynamic counter in the "Quick View" modal that automatically calculates pricing and links customers to a pre-filled WhatsApp message.
- **Menu Filter system**: Clean, lightweight Vanilla JS interactive category filters (All, Sweets, Snacks, Gift Boxes) without bloat.
- **Lead Capture & Inquiry Form**: Simple form for festival pre-orders, corporate gifting, and catering queries.
- **Embedded Interactive Map**: Highlights the central Kanpur location (Swaroop Nagar / Moti Jheel area).
- **Spring Boot & Thymeleaf Ready**: Pre-configured with Thymeleaf namespaces and placeholders (like `th:text`, `th:each`, `th:src`) for seamless integration into Java/Spring MVC projects. Works seamlessly in static preview.

---

## 🛠️ Tech Stack

- **Structure**: Semantic HTML5
- **Styling**: Tailwind CSS v3 (via Play CDN)
- **Icons**: Lucide Icons (via CDN)
- **Interactivity**: Vanilla JavaScript (no jQuery or heavy frameworks)
- **Backend Ready**: Spring Boot Thymeleaf (Visual Mockup compatible)

---

## 📁 Project Structure

```
kanpur_sweet_house/
│
├── images/               # High-end generated visual assets for the demo
│   ├── hero_sweets.png   # Assorted signature sweets box
│   ├── kaju_katli.png    # Kaju Katli (Cashew Fudge) close-up
│   ├── desi_ghee_laddu.png# Motichoor Laddu close-up
│   ├── special_samosa.png# Spiced Punjabi Samosa close-up
│   └── gift_box.png      # Festive gift box mockup
│
├── index.html            # Main single-page HTML template (Tailwind, JS, Thymeleaf)
├── .gitignore            # Git ignore configurations
└── README.md             # Project documentation
```

---

## 🚀 How to Run Locally

Since this is a static single-page template, no build process or local server is strictly required. 

1. Clone or download this repository.
2. Open `index.html` directly in any web browser (Chrome, Firefox, Safari, Edge).
3. Alternatively, serve it using any simple local server (e.g., Live Server extension in VS Code, or `python -m http.server 8000`).

---

## 🍃 Thymeleaf Integration (For Spring Boot Developers)

This template is fully prepared for Spring Boot Thymeleaf engines. Standard HTML values serve as static fallback content, while `th:` tags enable dynamic data rendering on the server:

- **Looping Items (`th:each`)**: Features `th:remove="all-but-first"` on parent grid containers, enabling you to test the loop with a single template element in production while retaining multiple mockup cards during static preview.
- **Text Replacements (`th:text`)**: Automatically updates store name, contact numbers, address, and descriptions.
- **Dynamic Attributes (`th:attr`)**: Passes dynamic product information to the Vanilla JS modal controller.
