# 📬 Awesome Sales Email Tracking & Read Receipts 👁️‍🗨️

<p align="center">
  <img src="assets/banner.svg" alt="Awesome Sales Email Tracking &amp; Read Receipts Banner" width="100%" />
</p>

<p align="center">
  <a href="https://github.com/ishandutta2007/Awesome-Sales-Email-Tracking-Read-Receipts/stargazers"><img src="https://img.shields.io/github/stars/ishandutta2007/Awesome-Sales-Email-Tracking-Read-Receipts?style=social" alt="GitHub Stars" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Sales-Email-Tracking-Read-Receipts/network/members"><img src="https://img.shields.io/github/forks/ishandutta2007/Awesome-Sales-Email-Tracking-Read-Receipts?style=social" alt="GitHub Forks" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Sales-Email-Tracking-Read-Receipts/issues"><img src="https://img.shields.io/github/issues/ishandutta2007/Awesome-Sales-Email-Tracking-Read-Receipts?color=blue" alt="GitHub Issues" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Sales-Email-Tracking-Read-Receipts/blob/main/LICENSE"><img src="https://img.shields.io/github/license/ishandutta2007/Awesome-Sales-Email-Tracking-Read-Receipts?color=green" alt="License" /></a>
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome" />
</p>

---

> 🚀 **A curated directory of top SaaS sales engagement platforms, lightweight browser extensions, and open-source self-hosted email tracking infrastructure.** Master email observability, open pixel detection, link click tracking, Apple Mail Privacy Protection (MPP) defense, and CRM read receipts.

---

## 📑 Table of Contents

- [📈 Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [🏢 SaaS & Hosted Platforms](#-saas--hosted-platforms)
- [💻 Open-Source GitHub Projects](#-open-source-github-projects)
  - [⭐ Open-Source Leaderboard (Sorted by Stars)](#-open-source-leaderboard-sorted-by-stars)
  - [📦 Project Deep-Dives](#-project-deep-dives)
- [🛡️ The Apple MPP & Tracking Pixel Reality](#️-the-apple-mpp--tracking-pixel-reality)
- [🤝 How to Contribute](#-how-to-contribute)
- [⚖️ Disclaimer & Privacy Compliance](#️-disclaimer--privacy-compliance)

---

## 📈 Sector Overview & Market Dynamics

The global **Sales Engagement Platform (SEP) & Email Tracking market** is valued at approximately **$7.5B to $9.2B**, expanding at a rapid **CAGR of ~15%** toward an estimated $30B+ by 2033. The niche dedicated to sales email tracking, sequencing, and inbox deliverability telemetry represents a $1.3B+ specialized subsegment.

**Market Concentration & Fragmentation**:
The sector is **moderately to highly fragmented**. While mega-cap revenue orchestration platforms (HubSpot, Salesforce, Outreach, Salesloft) command enterprise contract volume, the space resists a pure "winner-take-all" outcome due to low barriers to building pixel-injecting extensions, strong bottom-up Product-Led Growth (PLG) adoption among sales reps, and continuous protocol disruptions (such as Apple's Mail Privacy Protection and stricter Google/Yahoo bulk sender rules) which reward agile startups and self-hosted privacy engines.

---

## 🏢 SaaS & Hosted Platforms

Below is an audited comparison of leading commercial email tracking and sales engagement tools, sorted descending by **Company Scale (Market Cap / Valuation / ARR)**:

| Product | Company Scale (Valuation / Revenue) 🏢 | Pricing (Starting Paid Tier) 💳 | Free Tier / Trial Limit 🎁 | Key Capabilities 🛠️ |
| :--- | :--- | :--- | :--- | :--- |
| **[HubSpot Sales Hub](https://www.hubspot.com/)** | **~$21B - $35B** Market Cap / **$3.1B+** ARR | **$15/user/month** (Starter tier billed annually, or $20 billed monthly) | **Free Forever Plan**: Capped at 2 user seats, 1,000 contacts, 3 templates, 3 snippets, and 1 personal meeting link (HubSpot branding on sent emails). | Enterprise CRM-native open/click notifications, email templates, sequences, call tracking, and pipeline intelligence. |
| **[Outreach](https://www.outreach.io/)** | **~$4.4B - $5.0B** Valuation / **~$300M+** ARR | **$100/user/month** (Standard starting enterprise seat, billed annually) | **No Free Tier**: Demo/sales-qualified enterprise pilot only (no self-serve free trial). | Enterprise sales execution platform with multivariant cadences, engagement tracking, conversation AI, and pipeline analytics. |
| **[Salesloft](https://salesloft.com/)** | **~$2.3B** Valuation (Merged w/ Clari for **~$450M** combined ARR) | **$125/user/month** (Essential/Advanced tier base seat estimate, annual agreement) | **14-day Free Trial**: Full feature access trial requiring sales onboarding (no permanent free tier). | AI-driven revenue orchestration, cadences, real-time email engagement alerts, dialer, and deal forecasting. |
| **[Bananatag](https://bananatag.com/)** *(Staffbase Email)* | **~$1.1B** Valuation *(Staffbase Unicorn)* / **~$100M+** ARR | **$8/user/month** (Staffbase Email package base estimate, billed annually) | **No Free Tier**: 14-day assisted enterprise pilot upon demo request. | Enterprise internal email communications & sales tracking with detailed heatmaps, opens, click metrics, and Slack integration. |
| **[Mixmax](https://www.mixmax.com/)** | **~$60M - $100M** Est. Valuation / **~$15M** ARR | **$29/user/month** (SMB plan billed annually, or $34 monthly) | **Free Forever Plan**: Capped at 20 tracked emails/month, sequences capped at 50 recipients/month, and includes meeting polls. | Gmail & Outlook productivity layer offering instant notifications, custom sequences, in-email interactive polls, and calendar links. |
| **[Yesware](https://www.yesware.com/)** | **~$50M** Acquisition *(by Vendasta)* / **~$14M** ARR | **$15/user/month** (Pro plan billed annually, or $19 monthly) | **Free Forever Plan**: Capped at 10 campaign recipients/month, basic open tracking, and 1 meeting scheduler link. | Sales email tracking for Gmail & Outlook with presentation attachment view analytics, merge campaigns, and Salesforce auto-sync. |
| **[Streak](https://www.streak.com/)** | Bootstrapped / **~$8M - $10M** ARR | **$49/user/month** (Pro plan billed annually, or $59 monthly) | **Free Forever Plan**: Capped at 500 tracked emails/month, 200 total CRM contacts, and mail merge up to 50 recipients. | Complete CRM residing natively inside Gmail inbox; track email opens, log thread history, and advance deal pipelines seamlessly. |
| **[Boomerang](https://www.boomeranggmail.com/)** | Bootstrapped / **~$8M** ARR | **$4.98/month** (Personal plan billed annually, or $14.98/mo for Pro) | **Free Forever Plan**: Capped at 10 message credits per month (credits apply to Send Later, read receipts, and reminders). | Pioneering Gmail & Outlook extension for read receipts, follow-up nudges, snooze inbox, and AI writing assistance (*Respondable*). |
| **[GMass](https://www.gmass.co/)** | Bootstrapped / **~$8.5M** ARR | **$29.95/month** (Standard plan for 1 Google account) | **7-day Free Trial**: Strictly capped at 50 emails per day (all free tiers eliminated). | Mass email service and mail merge inside Gmail; automatic follow-up campaigns, open and click rate telemetry, and bounce management. |
| **[Mailtrack](https://mailtrack.io/)** *(Mailsuite)* | Bootstrapped / **~$4.8M** ARR | **$2.99/user/month** (Advanced plan billed annually, or $9.99 monthly) | **Free Forever Plan**: Unlimited email open and click tracking with mandatory *"Sent with Mailtrack"* signature branding appended. | Ultra-lightweight Gmail read receipt extension providing WhatsApp-style double checkmarks (`✓✓`) upon message open. |

---

## 💻 Open-Source GitHub Projects

Open-source email tracking infrastructure offers self-hosted data ownership, zero seat-licensing fees, and verifiable telemetry privacy. Below is the curated leaderboard sorted descending by GitHub community popularity:

### ⭐ Open-Source Leaderboard (Sorted by Stars)

| Repository | GitHub Stars Badge 🌟 | Tech Stack 🛠️ | Description 📝 |
| :--- | :--- | :--- | :--- |
| **[apparition47/MailTrackerBlocker](https://github.com/apparition47/MailTrackerBlocker)** | [![Stars](https://img.shields.io/github/stars/apparition47/MailTrackerBlocker?style=social&color=white)](https://github.com/apparition47/MailTrackerBlocker/stargazers) | Objective-C / Swift | Apple Mail tracker and spy-pixel blocker plugin that strips tracking pixels and blocks telemetry requests. |
| **[marckohlbrugge/sessy](https://github.com/marckohlbrugge/sessy)** | [![Stars](https://img.shields.io/github/stars/marckohlbrugge/sessy?style=social&color=white)](https://github.com/marckohlbrugge/sessy/stargazers) | TypeScript / Svelte | Open-source email delivery and observability dashboard for AWS SES; tracks sends, opens, clicks, bounces, and complaints. |
| **[tomer8007/whatsapp-web-incognito](https://github.com/tomer8007/whatsapp-web-incognito)** | [![Stars](https://img.shields.io/github/stars/tomer8007/whatsapp-web-incognito?style=social&color=white)](https://github.com/tomer8007/whatsapp-web-incognito/stargazers) | JavaScript / Chrome Ext | Browser extension blocking read receipts, presence status, and typing indicators with detailed receipt logs. |
| **[OCA/social](https://github.com/OCA/social)** | [![Stars](https://img.shields.io/github/stars/OCA/social?style=social&color=white)](https://github.com/OCA/social/stargazers) | Python / Odoo | Odoo community module suite featuring `mail_tracking` for native CRM chatter read receipts and open detection. |
| **[OneClickLab/ugly-email-extension](https://github.com/OneClickLab/ugly-email-extension)** | [![Stars](https://img.shields.io/github/stars/OneClickLab/ugly-email-extension?style=social&color=white)](https://github.com/OneClickLab/ugly-email-extension/stargazers) | JavaScript / Chrome Ext | Detects and blocks email tracking pixels and read receipt triggers in Gmail before they phone home. |
| **[trockerapp/trocker](https://github.com/trockerapp/trocker)** | [![Stars](https://img.shields.io/github/stars/trockerapp/trocker?style=social&color=white)](https://github.com/trockerapp/trocker/stargazers) | JavaScript / Firefox Ext | Browser extension that neutralizes tracking pixels, unshortens tracking links, and exposes tracking attempts. |
| **[brampauwelyn/php-email-tracker](https://github.com/brampauwelyn/php-email-tracker)** | [![Stars](https://img.shields.io/github/stars/brampauwelyn/php-email-tracker?style=social&color=white)](https://github.com/brampauwelyn/php-email-tracker/stargazers) | PHP / MySQL | Lightweight standalone tracking pixel server; serves 1×1 transparent GIF and records open timestamps, IP, and user-agent. |
| **[kJamesy/Laravel4-Newsletter-Application](https://github.com/kJamesy/Laravel4-Newsletter-Application)** | [![Stars](https://img.shields.io/github/stars/kJamesy/Laravel4-Newsletter-Application?style=social&color=white)](https://github.com/kJamesy/Laravel4-Newsletter-Application/stargazers) | PHP / Laravel | Newsletter dispatch and campaign management engine with automated open pixel tracking and link redirects. |
| **[leavemealone-app/email-trackers](https://github.com/leavemealone-app/email-trackers)** | [![Stars](https://img.shields.io/github/stars/leavemealone-app/email-trackers?style=social&color=white)](https://github.com/leavemealone-app/email-trackers/stargazers) | JSON / Rules | Curated blocklist and signature dataset of commercial email tracking URLs and spy-pixel patterns. |
| **[prashantsengar/mTracker](https://github.com/prashantsengar/mTracker)** | [![Stars](https://img.shields.io/github/stars/prashantsengar/mTracker?style=social&color=white)](https://github.com/prashantsengar/mTracker/stargazers) | Python / Flask | Flask web service for generating custom email tracking pixels with real-time open notification alerts. |
| **[kortirso/emailbutler](https://github.com/kortirso/emailbutler)** | [![Stars](https://img.shields.io/github/stars/kortirso/emailbutler?style=social&color=white)](https://github.com/kortirso/emailbutler/stargazers) | Ruby / Rails Engine | Rails engine tracking email dispatch status, delivery receipts, opens, and bounce/resend handling. |
| **[CurryOnPatat/mail-php-tracking-with-gui](https://github.com/CurryOnPatat/mail-php-tracking-with-gui)** | [![Stars](https://img.shields.io/github/stars/CurryOnPatat/mail-php-tracking-with-gui?style=social&color=white)](https://github.com/CurryOnPatat/mail-php-tracking-with-gui/stargazers) | PHP / Webhook | GUI email tracker logging opens with IP, device, and dispatching real-time notifications via Telegram & Discord webhooks. |
| **[civiccc/opentrak](https://github.com/civiccc/opentrak)** | [![Stars](https://img.shields.io/github/stars/civiccc/opentrak?style=social&color=white)](https://github.com/civiccc/opentrak/stargazers) | Ruby / Sinatra | Minimalist pixel tracking endpoint built on Sinatra with Redis caching for ultra-low latency pixel delivery. |
| **[we4tech/golang-email-tracker](https://github.com/we4tech/golang-email-tracker)** | [![Stars](https://img.shields.io/github/stars/we4tech/golang-email-tracker?style=social&color=white)](https://github.com/we4tech/golang-email-tracker/stargazers) | Go / Gin | High-performance Go microservice providing open telemetry and read confirmation webhooks. |
| **[wrfly/et](https://github.com/wrfly/et)** | [![Stars](https://img.shields.io/github/stars/wrfly/et?style=social&color=white)](https://github.com/wrfly/et/stargazers) | Go / SQLite | Self-hosted email tracker generating on-demand 1×1 PNG pixel links with automated email read notifications. |
| **[saranshdhingra/zmt](https://github.com/saranshdhingra/zmt)** | [![Stars](https://img.shields.io/github/stars/saranshdhingra/zmt?style=social&color=white)](https://github.com/saranshdhingra/zmt/stargazers) | Python / Flask | Specialized tracker integrating with Zoho Mail client for outbound email read receipts. |
| **[SohamRatnaparkhi/email-tracker-go](https://github.com/SohamRatnaparkhi/email-tracker-go)** | [![Stars](https://img.shields.io/github/stars/SohamRatnaparkhi/email-tracker-go)](https://github.com/SohamRatnaparkhi/email-tracker-go/stargazers) | Go / Redis | High-concurrency tracking microservice with template variable substitution and expiring pixel keys. |
| **[Luciano655dev/OpenTrackMail](https://github.com/Luciano655dev/OpenTrackMail)** | [![Stars](https://img.shields.io/github/stars/Luciano655dev/OpenTrackMail?style=social&color=white)](https://github.com/Luciano655dev/OpenTrackMail/stargazers) | JavaScript / Chrome Ext | Transparent, privacy-oriented Chrome extension injecting inspectable tracking tokens into Gmail. |
| **[amardeep1306/mail-tracker](https://github.com/amardeep1306/mail-tracker)** | [![Stars](https://img.shields.io/github/stars/amardeep1306/mail-tracker?style=social&color=white)](https://github.com/amardeep1306/mail-tracker/stargazers) | Python / Flask / Firefox | Educational tracking pixel system pairing a Firefox Gmail injector with a Flask & SQLite analytics UI. |
| **[aayostem/hunter](https://github.com/aayostem/hunter)** | [![Stars](https://img.shields.io/github/stars/aayostem/hunter?style=social&color=white)](https://github.com/aayostem/hunter/stargazers) | TypeScript / ClickHouse | Full-stack engagement suite with isolated pixel ingestors, BullMQ queues, ClickHouse analytics, and AI follow-up scoring. |

---

### 📦 Project Deep-Dives

#### 🔬 Full-Featured Tracking Suites & Architecture
- **[hunter (aayostem)](https://github.com/aayostem/hunter)**: Complete architectural blueprint for self-hosted email observability. Decouples pixel ingest endpoints from the REST API, records high-volume events into **ClickHouse**, manages retry backpressure via **BullMQ**, and incorporates Hugging Face sentiment scoring.
- **[sessy (marckohlbrugge)](https://github.com/marckohlbrugge/sessy)**: Observability console designed specifically for teams using Amazon Simple Email Service (SES). Surfaces delivery metrics, reputation scores, read receipts, and click events with an embedded MCP server for AI agent workflows.

#### 🛡️ Privacy & Apple Mail Privacy Protection (MPP) Countermeasures
- **[EmailKnow](https://dev.to/shaojie/emailknow-an-honest-open-source-email-tracker-0-users-and-heres-the-whole-thing-edi)**: Built explicitly to solve Apple MPP pre-fetching corruption. Replaces deceptive binary checkmarks with four distinct states:
  - 🔥 **Clicked link** (verified human intent)
  - ✓✓ **Human open** (interactive client render)
  - ⚠️ **Apple/Proxy pre-load** (pre-cached on Apple/Google proxy servers; not flagged as a read)
  - ⧗ **Unknown**
- **[MailTrackerBlocker](https://github.com/apparition47/MailTrackerBlocker)** & **[Ugly Email](https://github.com/OneClickLab/ugly-email-extension)**: Essential client-side tools analyzing the opposing side of the email telemetry arms race by intercepting and disabling tracking beacons.

#### ⚡ Microservices & High-Speed Ingest Engines
- **[et (wrfly)](https://github.com/wrfly/et)** & **[email-tracker-go](https://github.com/SohamRatnaparkhi/email-tracker-go)**: Ultra-fast Golang microservices that serve lightweight 1×1 GIF/PNG assets in under 5ms, persisting read telemetry directly into Redis or SQLite.
- **[mail-php-tracking-with-gui](https://github.com/CurryOnPatat/mail-php-tracking-with-gui)**: Ideal for personal workflows; alerts sales representatives over Discord or Telegram immediately upon recipient interaction.

---

## 🛡️ The Apple MPP & Tracking Pixel Reality

Traditional email tracking relies on an embedded invisible `1×1` pixel image (`<img>`). When the recipient's mail client loads the image, the tracking server logs the recipient's IP address, time, and User-Agent.

> [!WARNING]
> **The Apple Mail Privacy Protection (MPP) Challenge:**  
> On iOS 15+, iPadOS 15+, and macOS Monterey+, Apple Mail routes remote content through a proxy network and **pre-caches all images immediately upon email delivery**—irrespective of whether the recipient ever viewed the email. Consequently:
> - Standard email trackers record an immediate false positive "Open" within seconds of delivery.
> - Open rates are inflated, and geolocation data points to Apple regional relay proxies.
> - Link click tracking (`HTTP 302` redirects) remains the only tamper-proof indicator of genuine human engagement.

---

## 🤝 How to Contribute

Contributions, tool submissions, and corrections are warmly welcomed!

1. 🍴 **Fork** this repository.
2. 🌿 Create a feature branch (`git checkout -b feature/new-tracker`).
3. ✏️ Add your platform or repository (ensure SaaS tools include explicit tier pricing and free limits; open-source projects must include the star badge).
4. 💾 Commit changes (`git commit -m "feat: add NewTracker to ecosystem"`).
5. 🚀 Push to branch and open a **Pull Request**.

---

## ⚖️ Disclaimer & Privacy Compliance

- **Legal Considerations**: Email tracking telemetry involves personal data processing (IP addresses, read timestamps). Users must comply with applicable data protection regulations, including the **GDPR (General Data Protection Regulation)**, **ePrivacy Directive**, and **CCPA/CPRA**, providing appropriate disclosures or consent where mandated.
- **Accuracy**: Metrics are directional estimates derived from public software directories, financial reports, and vendor documentation as of late 2026.

---

<p align="center">
  ⭐ <b>Star this repository if you find it valuable for sales engineering and email observability!</b> ⭐
</p>
