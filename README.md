# 🚕 Transport Plugin
### *Book your ticket. We handle the rest.*

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit%20Site-black?style=flat-square&logo=vercel)](https://transport-plugin.vercel.app)
&nbsp;
[![Hackathon](https://img.shields.io/badge/Built%20at-Hackathon%202026-blueviolet?style=flat-square)]()
&nbsp;
[![Made in](https://img.shields.io/badge/Made%20in-Baku%2C%20Azerbaijan-blue?style=flat-square)]()

---

## 🤔 Ever had this moment?

You just booked your flight. Confirmation email is in your inbox. You're ready.

Then you realize — *how am I actually getting to the airport?*

You open another app. Search your address. Check the price. Book a separate ride. Set a reminder.

**That's 5 extra steps for something that should just happen automatically.**

---

## ✈️ What We Built

**Transport Plugin** connects your ticket to your taxi — instantly, automatically, without switching apps.

The moment you purchase a flight or train ticket, a smart widget appears and asks one simple question:

> *"You're arriving at Heydar Aliyev Airport at 17:00 — where are you heading next?"*

You type your destination. We find you a driver. Done.

- Flying **into** Baku? → Taxi from the airport to your door, ready when you land.
- Taking the **train out**? → Taxi to the station, scheduled 1 hour before departure.

No copy-pasting addresses. No mental math on timing. No extra apps.

---

## 🎬 See It in Action

> Click **"Purchase Ticket"** on any ticket in the demo — watch what happens next.

**[→ Live Demo](https://your-deployment.vercel.app)**

We built demos for two real Azerbaijani transport providers:

| | Provider | Route |
|---|---|---|
| ✈️ | **AZAL Airlines** | Istanbul → Baku |
| 🚆 | **ADY Railways** | Baku → Ganja |

---

## 💥 Why It Matters

Every day, thousands of people in Azerbaijan land at GYD airport or walk out of Baku's railway terminal with no ride arranged. They stand at the exit, open Bolt or another app, and wait.

We think the ticket booking experience shouldn't end at the ticket. It should take you all the way home.

This plugin is a **bridge** — it sits between any booking platform and any ride service and makes them talk to each other, automatically.

---

## 🔌 For Developers

Any booking platform can plug this in with literally two lines:

```html
<!-- 1. Add the script -->
<script src="plugin.js"></script>
```

```javascript
// 2. Fire this event after a successful purchase
window.dispatchEvent(new CustomEvent('ticketPurchased', {
  detail: {
    venueName:  'Heydar Aliyev Airport',
    eventTime:  '17:00',
    ticketType: 'arrival' // or 'departure'
  }
}));
```

The plugin handles language detection, UI, driver matching, and scheduling automatically.

Works in **Azerbaijani, Russian, and English** — auto-detected from the browser.

---

## 🛠️ Built With

- Vanilla JavaScript — no frameworks, no dependencies
- Runs on any website, embedded in one script tag
- Deployed on Vercel

---

## 👥 The Team

| Name | Role |
|---|---|
| [Your Name] | Development |
| [Teammate] | Design |
| [Teammate] | Idea & Pitch |

---

## 🚀 What's Next

If we had more time, we'd connect this to real taxi APIs (Bolt, local providers), add live driver tracking on a map, and reach out to AZAL and ADY directly to integrate for real.

The plugin is ready. The idea is proven. The only thing left is the partnership.

---

*Built with ☕ in 24 hours · Baku, Azerbaijan*
