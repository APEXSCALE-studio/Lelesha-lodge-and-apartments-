# Lelesha Lodge & Apartments — Website

> A single-file hospitality demo site built for **Lelesha Lodge & Apartments**, Chimwala Road, Lusaka, Zambia.

![HTML](https://img.shields.io/badge/HTML5-single--file-c9a84c?style=flat-square&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-embedded-c9a84c?style=flat-square&logo=css3&logoColor=white)
![JS](https://img.shields.io/badge/JavaScript-vanilla-c9a84c?style=flat-square&logo=javascript&logoColor=white)
![Deploy](https://img.shields.io/badge/Deploy-GitHub%20Pages-c9a84c?style=flat-square&logo=github&logoColor=white)

---

## Overview

A fully responsive, dark-luxury hospitality website built as a client demo. Everything lives in a single `lelesha-lodge.html` file — no frameworks, no build tools, no dependencies beyond Google Fonts.

The site uses real photos supplied by the client and is designed to convert visitors into direct bookings via WhatsApp and email, bypassing third-party booking platforms.

---

## Live Demo

```
https://<your-username>.github.io/<repo-name>/lelesha-lodge.html
```

---

## Features

### Design
- Dark earth-tone luxury aesthetic — `#1a1510` base, gold (`#c9a84c`) accents
- **Cormorant Garamond** (serif, headings) + **Jost** (sans-serif, body)
- Grain texture overlay for depth
- Hero zoom animation on load
- Scroll-reveal animations on cards and feature blocks

### Sections
| Section | Description |
|---|---|
| **Hero** | Full-viewport pool photo with animated headline and dual CTAs |
| **Amenities Strip** | 6-item icon bar — pool, WiFi, parking, restaurant, conferencing, pet-friendly |
| **About** | Property story, overlapping image pair, and stat highlights |
| **Rooms** | 3 room cards (Standard, Deluxe, Self-Catering Apartment) with pricing and booking links |
| **Amenities** | 8-tile grid covering all facilities |
| **Conferencing** | Corporate events pitch with feature breakdown |
| **Gallery** | Asymmetric 6-image grid using real property photos |
| **Testimonials** | 3 guest review cards |
| **Book** | Dual-channel booking form (WhatsApp + Email) |
| **Map** | Embedded Google Maps with property pin |
| **Footer** | Links, contact details, copyright |

### Booking System
- Form pre-selects room type when "Check Availability" is clicked on a room card
- **WhatsApp** button sends a pre-filled message to `+260 97 376 6129`
- **Email** button opens a pre-filled mailto to `apexscale86@gmail.com`
- Client-side validation before either channel fires

### Navigation
- Fixed top nav with blur-on-scroll effect
- Desktop: full link bar with gold "Book Now" CTA
- Mobile: hamburger → full-screen drawer with large Cormorant links
- `scroll-padding-top: 70px` so anchors land below the fixed nav

### Mobile Optimisation
- Two breakpoints: tablet `≤900px` and mobile `≤480px`
- All multi-column grids collapse to single column
- `font-size: 1rem` on inputs prevents iOS auto-zoom
- Hero uses `min-height: 100svh` for correct Safari rendering
- Floating WhatsApp bubble (bottom-right) on mobile — always accessible
- `-webkit-appearance: none` on form controls removes iOS default styling
- `-webkit-font-smoothing: antialiased` for crisp text on OLED screens

---

## File Structure

```
repo/
├── lelesha-lodge.html        # Main site — all HTML, CSS, JS in one file
├── lelesha-pool1.jpg         # Hero image — pool with umbrella
├── lelesha-pool2.jpg         # Gallery — pool wide shot
├── lelesha-gate.jpg          # About — entrance gate
├── lelesha-exterior.jpg      # About — building exterior
├── lelesha-room-standard.jpg # Rooms — Standard Room
├── lelesha-room-deluxe.jpg   # Rooms — Deluxe Room
├── lelesha-room-studio.jpg   # Rooms — Self-Catering Apartment
├── lelesha-conference.jpg    # Conferencing section
├── lelesha-bar.jpg           # Gallery — bar & lounge
├── lelesha-restaurant.jpg    # Gallery — restaurant
├── lelesha-lounge1.jpg       # Gallery — living room
├── lelesha-lounge2.jpg       # Gallery — apartment lounge (wide banner)
├── lelesha-event.jpg         # Gallery — event table setup
└── README.md
```

---

## Deployment (GitHub Pages)

1. Create a new repository on GitHub
2. Upload all files (HTML + all `.jpg` images) to the root of the repo
3. Go to **Settings → Pages**
4. Set source to `main` branch, `/ (root)` folder
5. Click **Save** — your site will be live at:
   ```
   https://<username>.github.io/<repo-name>/lelesha-lodge.html
   ```

> All image `src` paths in the HTML are relative — they work locally and on GitHub Pages without any changes.

---

## Customisation Checklist

Before handing over to the client, swap out the following placeholders:

- [ ] `+260 97 376 6129` → client's real WhatsApp number (also in `wa.me` links)
- [ ] `apexscale86@gmail.com` → client's real email address
- [ ] Room pricing (`From K850`, `From K1,200`, `From K1,800`) → confirmed rates
- [ ] Check-in / Check-out times → confirm with client
- [ ] `© 2025` → update year if needed
- [ ] Google Maps embed URL → verify pin is accurate
- [ ] Testimonials → replace with real guest reviews if available

---

## Tech Stack

| Layer | Choice | Reason |
|---|---|---|
| Structure | HTML5 | Single-file, zero dependencies |
| Styling | CSS3 (embedded) | Custom properties, Grid, clamp(), animations |
| Scripting | Vanilla JS | No framework overhead |
| Fonts | Google Fonts CDN | Cormorant Garamond + Jost |
| Booking | WhatsApp API + mailto | Direct channels, no third-party fees |
| Hosting | GitHub Pages | Free, fast, no server needed |

---

## Contact

Built by **ApexScale Studio** — Lusaka, Zambia
Web design & development for hospitality, legal, fitness, and services businesses.

---

*Demo site. All contact details and pricing are subject to confirmation by the client.*
