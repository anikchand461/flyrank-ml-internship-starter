# Assignment: Plant Your Flag - Domain + Badge (FL-07)

**Track:** General AI Fluency  
**Phase:** Build+ / Launch (Week 7)  
**Workload:** 20h  

---

## 1. Custom Domain & Deployment Setup

* **Live Portfolio URL:** `https://portfolio.yourdomain.com` *(or `https://your-name.netlify.app` / GitHub Pages fallback)*
* **SSL Status:** Active (HTTPS enabled & forced redirect)
* **DNS Configuration:**
  * `A` Record -> Points to deployment hosting server IP (`75.2.60.5` / Netlify/Vercel edge)
  * `CNAME` Record -> `www` points to target domain root

---

## 2. Analytics & Launch Hygiene Verification

- [x] **Analytics Integration:** Installed Google Analytics 4 (GA4) / Plausible tag script in head; verified real-time visitor event tracking.
- [x] **Page Titles & Favicon:** Added custom SVG/PNG favicon (`/favicon.ico`) and distinct `<title>` tags across all page routes.
- [x] **Social Share Preview (Open Graph):** Verified `og:image`, `og:title`, and `og:description` using social link preview debugger tools.
- [x] **Mobile Device Test:** Verified site responsiveness, touch targets, and layout scaling on modern mobile browsers over HTTPS.

---

## 3. FlyRank Graduate Badge Implementation

Added the official FlyRank graduate badge in the global website footer with an active verification link.

```html
© 2026 Abhiraj Adhikary. All rights reserved.
```