# Awesome-Sales-Email-Tracking-Read-Receipts

## Top Sales Email Tracking & Read Receipts Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Open Tracking, Link Clicks & Self-Hosted Email Observability*  

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Sales Email Tracking & Read Receipts**. These tools enable sales teams to know when prospects open emails, click links, and engage with outreach—turning blind sending into data-informed follow-up and helping reps prioritize the hottest leads.



**Examples** include HubSpot Email Tracking, Yesware, Mailtrack, Mixmax, Salesloft, Outreach, Bananatag, GMass, Streak, and Boomerang (the category leaders).



**Open-source emphasis**: Sales Email Tracking is a domain where open-source tooling is **fragmented but genuinely functional for basic open/click tracking**. The strongest active projects are **hunter** (a privacy-focused, full-stack email tracking suite with separate tracking ingestor, ClickHouse analytics, and AI features) , **EmailKnow** (a Gmail extension that distinguishes human opens from Apple Mail Privacy Protection pre-loads—a critical honesty feature most tools ignore) , and **mail-tracker** (a Flask + Firefox extension implementation of the tracking pixel pattern) . For Go developers, **et** and **email-tracker-go** provide lightweight tracking services with Redis storage . For Odoo users, the **OCA mail_tracking** module adds read receipts directly to chatter emails . The critical caveat: **Apple's Mail Privacy Protection has broken open tracking for a large share of recipients**—pixels fire on Apple's servers before the human opens the email, making "Read" unreliable—and only EmailKnow explicitly addresses this with honest signal classification .



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[HubSpot Email Tracking](https://www.hubspot.com/)**  

  Native email tracking within HubSpot Sales Hub; open and click notifications tied directly to contact records, with sequences and templates.



- **[Yesware](https://www.yesware.com/)**  

  Sales email tracking and engagement platform for Gmail and Outlook; open/click tracking, templates, campaigns, and CRM integration.



- **[Mailtrack](https://mailtrack.io/)**  

  Simple Gmail read receipt extension; double checkmarks for opens, with a free tier and paid plans for unlimited tracking.



- **[Mixmax](https://www.mixmax.com/)**  

  Email engagement platform with sequences, tracking, scheduling, and polls; positioned for individual reps and small teams.



- **[Salesloft](https://salesloft.com/)**  

  Sales engagement platform with email tracking, cadences, dialer, and conversation intelligence.



- **[Outreach](https://www.outreach.io/)**  

  Sales engagement platform with sequences, tracking, and revenue intelligence analytics.



- **[Bananatag](https://bananatag.com/)**  

  Email tracking and analytics platform (now part of Staffbase); provides open/click tracking and engagement insights for internal communications and sales.



- **[GMass](https://www.gmass.co/)**  

  Gmail-based mass email and tracking tool; open/click tracking, auto follow-ups, and mail merge for cold outreach.



- **[Streak](https://www.streak.com/)**  

  CRM inside Gmail with email tracking, send later, and pipeline management; the free tier includes tracking and CRM features .



- **[Boomerang](https://www.boomeranggmail.com/)**  

  Gmail extension for scheduling, reminders, and read receipts; free tier limited to 10 emails/month .



## Open-Source GitHub Projects



### Full-Featured Tracking Suites



- **[hunter (aayostem)](https://github.com/aayostem/hunter)**  

  The most architecturally complete open-source **email tracking and engagement suite** for individuals and small teams . Features: **separate tracking ingestor service** (pixel/click endpoint isolated from API), **event store separation** (ClickHouse for analytics, PostgreSQL for relational data), **queue-backed sends** via BullMQ for retries and backpressure, open/click tracking, and optional AI features (OpenAI GPT-4o, sentiment via Hugging Face, send-time model via scikit-learn) . Docker Compose deployment with Kubernetes/Terraform options. **Best for teams wanting a production-grade, privacy-focused tracking foundation**—but it is a suite requiring infrastructure management (Postgres, Redis, ClickHouse).



- **[EmailKnow](https://dev.to/shaojie/emailknow-an-honest-open-source-email-tracker-0-users-and-heres-the-whole-thing-edi)**  

  The **most honest open-source email tracker** for Gmail—explicitly built to address Apple Mail Privacy Protection's impact on open tracking . Instead of a single green checkmark, it sorts signals into **four states**: 🔥 clicked a link (strongest signal), ✓✓ human open (confident), ⚠️ **Apple/proxy pre-load** (pixel fired but might be a machine—labeled, not counted as "read"), and ⧗ unknown . Also closes the loop with **signal-driven follow-ups** ("read but no reply" gets a different nudge than "never opened") . **Privacy stance**: never reads email body/attachments, stores IP only as salted SHA-256 hash, minimal Google scopes (send + metadata only) . Runs entirely on Cloudflare's free tier. **Best for teams wanting honest tracking that doesn't lie about Apple pre-loads**—but it is early-stage (0 users as of the DEV post) and Gmail-only.



- **[mail-tracker (amardeep1306)](https://github.com/amardeep1306/mail-tracker)**  

  Open-source **email read tracking system** for Firefox + Gmail (Flask backend, SQLite) . Injects a **1×1 tracking pixel** into every composed email; when the recipient opens it, the server logs time, IP, and user agent, and updates status to "read." Includes a **web dashboard** showing tracked emails, subject/recipient, read/unread status, timestamps, and summary stats (open rates, average read time) . **Best for developers wanting a simple, understandable implementation of the tracking pixel pattern**—but it is a learning project (Firefox-only, requires ngrok for public access) rather than a production tool.



### Lightweight Tracking Services (API / Go)



- **[et (wrfly)](https://pkg.go.dev/github.com/wrfly/et)**  

  Open-source **email tracker in Go** (Apache-2.0) . Design: user submits their email address, server generates a **1×1 pixel PNG link** with a unique track ID, user inserts the link into the email, and when opened the server sends a **notification email** to the user . Features: resume stopped tasks, check task status by track ID, API endpoints, and rate limiting (10 tasks/day/IP, 5 emails per task) . **Best for developers wanting a minimal, single-purpose tracking service**—no dashboard, just pixel + notification.



- **[email-tracker-go (sohamratnaparkhi)](https://pkg.go.dev/github.com/sohamratnaparkhi/email-tracker-go)**  

  Open-source **Go email tracking service** using Redis for storage and Gin for HTTP . Features: send emails to multiple recipients (TO, CC, BCC), **pixel tracking** via `GET /pixel/:tracking_id`, status endpoint, HTML templates with variable substitution, and configurable tracking expiration . **Best for Go teams wanting a simple tracking API** to integrate into existing systems—no UI, no database beyond Redis.



### CRM-Integrated Tracking



- **[OCA mail_tracking (Odoo)](https://github.com/Vauxxo/social/tree/16.0/mail_tracking)**  

  Open-source **Odoo module** that adds email tracking status to chatter messages . Features: status icons for each notified partner (**Waiting, Sent, Delivered, Opened**, plus Error/Cc/No Email) ; configurable system parameter to **disable tracking pixels** globally if desired; tracking emails and events accessible in Settings > Technical . **Best for Odoo users** wanting read receipts integrated directly into their CRM chatter—but it is Odoo-specific and requires the OCA module installation.



### Additional Strong Open-Source Options



- **OpenTrackMail** — Free, open-source **Chrome extension** for email open tracking directly from your inbox; simple, lightweight, and inspectable source code (v0.1.2, September 2026) . **Best for users wanting a transparent, no-frills Chrome extension**—but it is minimal and Gmail-focused.

- **Zoho Mail Tracker (supernova13892/zmt)** — Open-source **Zoho Mail tracking** tool listed in AlternativeTo's email tracker alternatives . **Niche**—for Zoho Mail users, but demonstrates the pattern for client-specific tracking.

- **Sessy** — Open-source **email observability for AWS SES** (not sales tracking per se, but relevant for teams sending via SES); tracks deliveries, bounces, complaints, opens, and clicks, with an MCP server for AI agent access . **Best for SES users wanting observability**—not a sales engagement tool.



**Frameworks for building custom systems**: For a **production-grade tracking suite with analytics**, hunter provides the most complete architecture . For **honest tracking that handles Apple pre-loads**, EmailKnow . For **simple pixel-based tracking in Python/Flask**, mail-tracker . For **Go-based tracking services**, et or email-tracker-go . For **Odoo CRM integration**, OCA mail_tracking . No open-source project matches Yesware's **CRM sync and sequence automation** or Mailtrack's **polished Gmail UX**—those are commercial advantages.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Email tracking platforms handling recipient data must comply with applicable privacy regulations (GDPR, CCPA) and anti-spam laws; **tracking pixels and open data collection may require disclosure or consent** depending on jurisdiction.

- **Apple Mail Privacy Protection has fundamentally broken open tracking**—pixels fire on Apple's servers before the human opens the email, making "Read" unreliable for a large share of recipients . Most commercial tools show a confident "Read" anyway; **EmailKnow is the only open-source project that explicitly addresses this** with honest signal classification . Treat open rates as directional, not definitive.

- **Open-source email tracking is fragmented**—hunter provides a production suite , EmailKnow provides honest tracking , and mail-tracker/et/email-tracker-go provide simple implementations . However, **no open-source project matches Yesware's CRM sync or Mailtrack's Gmail UX**—organizations requiring polished sales engagement should evaluate commercial platforms.

- Verify license terms for commercial use; hunter is open-source (check repository) , et uses Apache-2.0 , and EmailKnow is open-source .



---



**Made for sales operations teams, developers building tracking infrastructure, and teams choosing their email engagement stack.**  

Let's make email tracking more open, but with clear eyes about the Apple pre-load problem that makes "Read" a lie in most tools.
