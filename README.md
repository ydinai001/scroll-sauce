# Shimmy Edits

Short-form video editing service for creators who want scroll-stopping content.

**Live Site:** https://adorable-zabaione-493e62.netlify.app/

## Service Overview

- **Price:** $40 per reel
- **Turnaround:** 3 days
- **Platforms:** Instagram Reels, TikTok

## Features

### Landing Page
- Hero section with animated phone mockup preview
- Service pricing and features breakdown
- Social proof with floating stat cards
- Mobile-responsive design

### Video Gallery Modal
- "See Examples" button opens gallery of sample edits
- 5 example clips with thumbnail previews
- Lazy loading (`preload="none"`) for fast page load
- ESC key and click-outside to close

### Live Chat (Tawk.to)
- Real-time chat widget in bottom-right corner
- "Let's Talk!" button in hero section opens chat
- Mobile app notifications for site owner
- No personal phone number exposed

### Payments
- Stripe checkout integration
- "Order Your First Reel" and "Get Started" buttons link to Stripe

### Social Links
- Instagram: [@shimmyedits](https://instagram.com/shimmyedits)
- TikTok: [@shimmyedits](https://tiktok.com/@shimmyedits)

## Project Structure

```
scroll-sauce/
├── index.html              # Main landing page (all-in-one HTML/CSS/JS)
├── assets/
│   ├── images/             # Photography and graphics
│   ├── icons/              # Icon assets
│   ├── videos/             # Example video clips (clip-1.mp4 to clip-5.mp4)
│   └── thumbnails/         # Video thumbnails for gallery (thumb-1.jpg to thumb-5.jpg)
├── docs/                   # Project documentation
│   ├── prd.md              # Product Requirements Document
│   └── architecture/       # Technical architecture docs
├── css/                    # External stylesheets (future)
└── js/                     # External scripts (future)
```

## Tech Stack

- **Frontend:** HTML5, CSS3, Vanilla JavaScript
- **Fonts:** Google Fonts (Syne, Space Mono)
- **Payments:** Stripe Checkout
- **Live Chat:** Tawk.to
- **Hosting:** Netlify
- **Video:** HTML5 video with thumbnail posters

## Third-Party Integrations

| Service | Purpose | Configuration |
|---------|---------|---------------|
| Stripe | Payment processing | Checkout link in buttons |
| Tawk.to | Live chat widget | Script in index.html |
| Netlify | Hosting & deployment | Auto-deploy from GitHub |

## Development

### Local Preview
```bash
# Open in browser
open index.html

# Or use a local server
python3 -m http.server 8000
```

### Deploy
Push to `main` branch - Netlify auto-deploys from GitHub.

Manual: Drag `index.html` and `assets/` folder to [Netlify Drop](https://app.netlify.com/drop).

## Configuration

### Tawk.to Chat
Widget script is at the bottom of `index.html`. To change accounts:
1. Go to [tawk.to](https://www.tawk.to)
2. Get new embed code
3. Replace script between `<!--Start of Tawk.to Script-->` comments

### Stripe Checkout
Payment links are hardcoded in:
- Hero "Order Your First Reel" button
- Header "Get Started" button

To update, search for `buy.stripe.com` in index.html.

## Recent Updates

### December 18, 2024
- Added Tawk.to live chat integration
- Added "Let's Talk!" button to hero section
- Generated video thumbnails for faster gallery loading
- Added `preload="none"` to videos for performance
- Removed WhatsApp buttons (replaced with Tawk.to)

### December 17, 2024
- Added video gallery modal with 5 example clips
- Fixed video thumbnail overlapping issues
- Added "See Examples" button to hero

## Status

- [x] Landing page design
- [x] Video gallery modal
- [x] Stripe payment integration
- [x] Live chat (Tawk.to)
- [x] Video thumbnails for performance
- [ ] HoneyBook workflow setup
- [ ] Service package configuration
- [ ] Intake questionnaire
- [ ] Contract template

---

*Last Updated: December 18, 2024*
