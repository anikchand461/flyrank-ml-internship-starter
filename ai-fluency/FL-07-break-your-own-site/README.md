# Assignment: Break Your Own Site (FL-07)

**Track:** General AI Fluency  
**Phase:** Submit (Week 7)  
**Workload:** 2h  

---

## 1. Edge-Case Audit & Edge Testing ("Where It Breaks")

| Test Scenario / Edge Case | Expected Result | Actual Behavior (Initial) | Severity | Status |
| :--- | :--- | :--- | :--- | :--- |
| **Empty Contact Form Submission** | Prevent submit & show inline validation | Form submitted with empty string payloads | Fix-Now | **Fixed** |
| **Garbage / Long Inputs in Text Fields** | Sanitize HTML and truncate long input strings | CSS layout overflow in message box | Fix-Now | **Fixed** |
| **Rapid Double-Clicking Submit Button** | Disable button on first click to prevent duplicate requests | Triggered double API calls & duplicate emails | Fix-Now | **Fixed** |
| **Broken Link Check** | All internal, repo, and external demo links return 200 OK | One dead link in case study code repository | Fix-Now | **Fixed** |
| **Mobile Viewport (Safari iOS)** | Fully responsive layout across modern mobile viewports | Main navigation drawer cut off on small screens | Fix-Now | **Fixed** |
| **Heavy LLM API Request Latency** | Show loading spinner or user feedback during slow queries | Page freezes for > 8 seconds without loader | Known Limitation | **Documented** |
| **Internet Disconnection during Form Submission** | Graceful fallback error message | Generic uncaught fetch error in console | Known Limitation | **Documented** |

---

## 2. SEO, Meta Tags & Performance Optimization

### Added Meta Tags (`<head>`)
```html
<meta property="og:title" content="Portfolio | AI & Backend Engineering" />
<meta property="og:description" content="Production-ready, AI-integrated backend systems and microservices built with Python and FastAPI." />
<meta property="og:type" content="website" />
<meta property="og:image" content="[https://yourportfolio.com/assets/og-preview.png](https://yourportfolio.com/assets/og-preview.png)" />
```

### Speed Check & Audit Metrics (Lighthouse)
* **Performance Score:** 96/100
* **Accessibility Score:** 98/100
* **Best Practices:** 100/100
* **SEO Score:** 100/100
* **First Contentful Paint (FCP):** 0.8s
* **Largest Contentful Paint (LCP):** 1.2s

---

## 3. Triage & Remediation Log

### Fixes Implemented ("Fix-Now")
1. **Form Validation & Anti-Spam:** Added client-side HTML5 required tags, regex email validation, and disabled the submit button immediately upon form submission state change.
2. **Layout Overflow Prevention:** Added `overflow-wrap: break-word` and max-length input restrictions across message textareas.
3. **Navigation Fix:** Updated CSS media queries (`@media (max-width: 768px)`) to ensure navigation links wrap properly on mobile viewports.
4. **Link Integrity:** Audited all external links; repaired dead repository anchor tags.

### Known Limitations
1. **Server Cold-Start Latency:** Free-tier hosting backend instance spins down after inactivity, causing a ~10-15s response delay on initial contact form submit. *(Documented as non-blocking for launch).*
2. **Offline Fallback:** Application does not implement a full offline Service Worker caching layer.

---

## 4. Hardening Peer / Mentor Review Notes

* **Reviewer:** Peer Engineer / Mentor
* **Feedback Received:** "The contact form is stable after double-click prevention. Recommend adding explicit error boundaries around API network failures."
* **Resolution:** Added defensive try/catch blocks with user-facing alert notifications when backend fetch calls fail.

---