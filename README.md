# 🎯 Job Candidate Application Tracker
> **Solving the Hiring Black Hole with Real-Time Transparency, Clear Timelines, and Candidate Agency.**

A clean, modern, single-page web application designed with a Linear/Stripe/Notion-inspired SaaS aesthetic. It gives candidates total visibility into their job application status, transparent next steps, guaranteed timelines, and direct recruiter access.

---

## ⚡ Quick Start & Deployment

### Option 1: GitHub Pages (Instant Zero-Build Deployment)
1. Push this folder to a GitHub repository (e.g., `job-candidate-tracker`).
2. Go to **Settings** → **Pages**.
3. Under **Build and deployment**, select **Source: Deploy from a branch** and choose branch `main` (folder `/root`).
4. Click **Save**. Your site will be live immediately at `https://<username>.github.io/<repo>/`!

### Option 2: Run Locally
- **Directly in Browser:** Double-click `index.html` to open it in any web browser.
- **Or via Local Web Server:**
  ```bash
  npx serve .
  # or
  python -m http.server 8000
  ```

---

## ✨ Key Features

1. **Demo Profile Switcher (Top Sticky Bar):**
   - **Candidate A (Sarah Chen - Senior Product Designer):** *Active — Action Required*. Needs to book an interview.
   - **Candidate B (Marcus Vance - Staff Frontend Engineer):** *Active — Waiting on Hiring Team*. Transparent review notice; no action required.
   - **Candidate C (Priya Nair - Senior Data Analyst):** *Completed — Offer Extended*. Full formal offer package ready for review and electronic acceptance.
   - **Application Lookup Modal:** Search by Application ID (`APP-8492`, `APP-7130`, `APP-9521`) or email with 1-click demo autofill.

2. **Visual Stage Progress Tracker:**
   - 5 Evaluation Stages: *Application Received* → *Resume Review* → *Hiring Manager Interview* → *Final Panel* → *Decision & Offer*.
   - Responsive layout: dynamic horizontal multi-step progress bar on desktop; clean vertical stepper on mobile devices.
   - Distinct visual cues for Completed (emerald checkmark), Current stage (pulsing indicator), and Upcoming stages.

3. **"What Happens Next" Action Hero Card:**
   - High-contrast, reassuring card answering the most anxious question candidates have: *"What is happening right now and what is expected of me?"*
   - Interactive CTAs:
     - **For Sarah Chen:** Interactive 30-min interview booking modal with date chips and time slots. Selecting a slot dynamically updates the candidate status to *Interview Confirmed*, adds an entry to the live Activity Log, and fires a celebration animation!
     - **For Marcus Vance:** Reassuring *"No action required"* card with SLA date commitment.
     - **For Priya Nair:** Interactive *Review & Accept Offer Package* modal displaying salary, equity, sign-on bonus, benefits, and an electronic sign button with full confetti effect.

4. **Timestamped Activity Log:**
   - Real-time audit trail of all candidate interactions, interview approvals, and status transitions.
   - New actions (scheduling calls, recruiter inquiries, accepting offers) append directly to the log in real time.

5. **Assigned Recruiter Contact & Inquiries:**
   - Recruiter avatar, direct email, average reply time indicator (< 2 hours).
   - "Send a Question" modal allowing candidates to ask timeline questions, provide updated portfolio/github links, or alert the team about competing offers.

6. **Candidate Dignity & Zero-Ghosting SLA:**
   - 5-business-day response guarantee policy modal.
   - FAQ accordion addressing key candidate concerns (deadlines, resume updates, constructive feedback).
   - Clean printable layout (`window.print()` / PDF export friendly).

---

## 🛠️ Tech Stack & Constraints Met
- **HTML5 & Vanilla JavaScript:** 100% self-contained in a single file with zero compilation, Node.js, or backend requirements.
- **Tailwind CSS (via CDN):** Clean typography (Plus Jakarta Sans & JetBrains Mono), calm color palette, and micro-interactions.
- **Lucide Icons & Canvas Confetti (via CDN):** Crisp vector icons and celebratory visual feedback.
