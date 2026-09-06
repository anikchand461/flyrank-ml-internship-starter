# Assignment: Draw the Path (Portfolio Sitemap + Toolkit)

**Track:** General AI Fluency  
**Phase:** Setup (Week 1)  

---

## 1. Portfolio Proof Statement & Core Action

* **Target Audience ("One Person"):** Technical Recruiters & Engineering Leads hiring AI/Backend Engineers.
* **Core Claim / Proof Statement:** "I build production-ready, AI-integrated backend systems and scalable microservices with clean, testable code."
* **The One Action:** Book a intro call or submit a contact inquiry to discuss backend/AI engineering roles.

---

## 2. Portfolio Sitemap

```text
[ Landing / Hero ] ---> [ Case Studies / Proof ] ---> [ About Me ] ---> [ Contact / CTA ]
```


* **Page 1: Landing (Hero)**
  * *Purpose:* Immediately presents the core claim, highlights top technical stacks (Python, FastAPI, Docker, LLMs), and directs visitors to the case studies or contact form.
* **Page 2: Case Studies / Selected Projects**
  * *Purpose:* Displays 2-3 deep-dive technical projects proving the core claim through architecture diagrams, code repos, and measurable metrics.
* **Page 3: About**
  * *Purpose:* Brief background on technical skills, engineering philosophy, and links to GitHub / LinkedIn.
* **Page 4: Contact**
  * *Purpose:* Simple form and direct email/booking link executing **The One Action**.

---

## 3. Toolkit Accounts Setup

- [x] **Claude** (Active)
- [x] **ChatGPT** (Active)
- [x] **Gemini** (Active)
- [x] **Perplexity** (Active)

---

## 4. Claude Project Configuration

* **Project Name:** `Portfolio Build & AI Fluency Tutor`
* **Custom Instructions:**
  > "You are an expert technical portfolio coach and senior backend engineering tutor. You are helping me build my personal portfolio over the next 8 weeks.
  > 
  > Core Claim: 'I build production-ready, AI-integrated backend systems and scalable microservices with clean, testable code.'
  > Core Action: Convince technical recruiters and engineering leads to book an intro interview.
  > 
  > Tone & Guidance Style:
  > - Direct, constructive, and hyper-focused on efficiency and scannability.
  > - Pressure-test every portfolio decision against my Core Claim and Core Action.
  > - Help refine code examples, system architecture diagrams, and technical write-ups."

---

## 5. Pressure-Test Prompt & AI Feedback

### Prompt Used:
> "Act as a senior backend engineering recruiter. Review my proposed 4-page portfolio sitemap (Hero/Landing, Case Studies, About, Contact) against my Core Claim: 'I build production-ready, AI-integrated backend systems and scalable microservices with clean, testable code' and my Core Action (getting engineering leads to book an intro call). Pressure-test this setup: Are there any redundant pages? What missing element could prevent a visitor from taking the core action?"

### Claude Feedback Summary:
1. **Sitemap Evaluation:** The 4-page structure is lean and direct. No unnecessary fluff pages (like blog archives or long galleries).
2. **Key Flaw Identified:** Having "Contact" as a separate page introduces unnecessary friction. A recruiter might view the case study and leave before clicking to a standalone Contact page.
3. **Actionable Revision Made:** Embed a direct "Book a Call / Contact" section directly at the bottom of the Landing page and at the end of every Case Study page, while keeping a clean dedicated `/contact` URL anchor for direct navigation.

---