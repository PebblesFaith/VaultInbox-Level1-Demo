VaultInbox is a digital certified delivery platform that replaces USPS Certified Mail with a faster, cheaper, and more secure alternative. Each message generates a unique Tracking ID and tamper-evident audit log, providing court-admissible proof of delivery under ESIGN/UETA. Unlike legacy mail or bulky e-sign platforms, VaultInbox integrates directly with existing email addresses, giving users instant, verifiable delivery at a fraction of the cost.

# VaultInbox

**Digital Certified Delivery Simplest Prototype Example — Reinvented for the Email Era**

---

## The Problem

Every year, businesses and individuals spend **billions** on USPS Certified Mail and courier services just to prove that a critical document was sent, received, and opened.
This legacy system is:

* **Slow** — delivery takes days, not seconds.
* **Expensive** — \$7–\$10 per Certified Mail piece (plus staff handling).
* **Inefficient** — requires in-person handling, return receipts, and manual filing.
* **Risk-prone** — mail theft and lost items remain common.

In today’s digital world, organizations need **court-admissible proof of email delivery** — faster, cheaper, and more secure than physical certified mail.

---

## The Solution: VaultInbox

VaultInbox is a **digital certified delivery platform** that provides the functional equivalent of USPS Certified Mail **inside email workflows**.

* **Proof of Delivery:** Every message generates a unique **Tracking ID (UUID)** and a tamper-evident audit log.
* **Court Admissibility:** Audit artifacts are timestamped, cryptographically verifiable, and aligned with **ESIGN / UETA** standards.
* **Seamless Adoption:** Works with **users’ existing email addresses** — no new inbox or migration required.
* **Instant Delivery:** From sender to recipient in seconds, not days.
* **Cost Efficiency:** Pricing is positioned at a fraction of USPS Certified Mail, enabling massive enterprise savings.

---

## How It Works

1. **Compose** – Sender attaches a PDF/document and sends via VaultInbox.
2. **Tracking** – The recipient journey (SENT → DELIVERED → OPENED → CLOSED) is logged in real time.
3. **Proof** – VaultInbox generates a **verifiable certificate (PDF)** with delivery artifacts.

Investors can preview this **flow in our Level-1 Demo**: a safe, static prototype that walks through the VaultInbox user experience without exposing backend code.

---

## Market Opportunity

* **USPS Certified Mail Volume:** \~**150–200M pieces annually** in the U.S. alone.
* **Cost per Piece:** \$7–\$10 (all-in).
* **Market Size:** \$1.2B+ annual spend in the U.S., larger globally.
* **Digital Transition:** Enterprises, law firms, healthcare providers, and government agencies increasingly seek **digital-first certified delivery**.

Even capturing **5% of USPS Certified Mail volume** digitally represents a **\$60M+ annual revenue opportunity**.

---

## Competitive Advantage

* **USPS Alternative:** Direct digital equivalent of Certified Mail with stronger fraud protection.
* **Simplicity:** Users continue to use their existing email addresses. No new domain or inbox to manage.
* **Security:** Powered by **AccouNetrics Lockbox Protocol** (provisional patent filed June 2025), ensuring session integrity and audit log immutability.
* **Cost & Speed:** Sub-second delivery at a fraction of the cost of USPS or competitors.
* **Focus:** Unlike e-signing platforms (e.g., DocuSign, RMail, RDocs), VaultInbox is **laser-focused on certified delivery**, not general contract execution.

---

## Traction & Roadmap

* **Prototype:** Level-1 Demo (investor-safe static walk-through).
* **Engineering Build (Level-2):** Full Express + SQLite + Mailer app (internal).
* **Next Steps:**

  * Add enterprise integrations (Outlook, Gmail, APIs).
  * Launch beta with legal, healthcare, and financial services firms.
  * Scale to subscription model (\$20/user/month) with transactional pricing.

---

## Why Now

* Mail theft, fraud, and delays are rising.
* Courts increasingly accept **digital delivery proofs** under ESIGN/UETA.
* Enterprises demand **faster, cheaper, and greener** certified communication.

VaultInbox delivers the **right solution at the right time** — a modern SaaS platform for a multi-billion-dollar legacy market.

---

## Contact

**VaultInbox (Powered by AccouNetrics)**
📧 [contact@vaultinbox.cloud](mailto:contact@vaultinbox.cloud)
🌐 [vaultinbox.cloud](#)

---



# AccouNetrics v0.1.7d — UUID-as-Primary-Key

## Changes
- `users.id` is now **TEXT UUID** with a SQLite **DEFAULT** expression (auto-generated).
- All foreign keys updated to TEXT.
- Seeds from `seed_users` (visible in migration) — DB auto-generates UUIDs.
- USPS features + Email management intact.
- Header shows account #: user.id

## Run
```bash
npm install
npm start
# open http://localhost:3000
```

## Reset DB
```bash
rm -f data/accounetrics.db
npm start
```
