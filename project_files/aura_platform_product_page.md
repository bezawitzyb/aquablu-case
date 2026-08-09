# AURA — Aquablu's Hydration Platform (Product-Page Edition)
### Research file for Bezawit Zerayacob Bekele · Digital Product Builder · August 2026

> This file is built primarily from Aquablu's **official AURA product page** (aquablu.com/products/aura), cross-referenced with the REFILL+ Series 2 launch, the BOLD/CES 2026 release, and Aquablu's Service Terms. Where a claim comes from the product page it's stated plainly; where it's from other sources or is inference, that's flagged. A companion file (the earlier "AURA deep dive") covers the three-layer architecture and strategic flywheel in more depth — this one is the tighter, marketing-accurate version you can quote from safely.

---

# AURA — Deep Dive on Aquablu's Hydration Operating System
### Research brief for Bezawit Zerayacob Bekele · Digital Product Builder interview prep · August 2026

---

## 1. What AURA Is, in One Breath

AURA is Aquablu's **"Hydration Operating System"** — the software and data platform launched alongside the REFILL+ Series 2 on **7 October 2025**. Aquablu describes it as the platform that "connects all Aquablu products and data into one intelligent ecosystem." It is the connective tissue between three worlds: the **physical dispensers** (REFILL+ Series 2, BOLD), the **people who drink from them** (~150,000 daily users), and the **people who operate them** (facility managers, partners, and Aquablu's own service/logistics teams).

The company's own framing (from the Series 2 press release): *"The real breakthrough, and a major step toward data-driven facility management, is AURA — the new Hydration Operating System that connects all Aquablu systems and data in one smart dashboard."*

**Why it matters for your interview:** the Digital Product Builder job description defines the digital portfolio as "AURA in users' hands, our dispenser's digital surfaces, and the platform connecting hundreds of deployed systems." AURA *is* the product surface this role owns a slice of.

---

## 2. Architecture: The Three Layers of AURA

Piecing together the press releases, product pages, founder interviews, and job ads, AURA operates across three layers:

### Layer 1 — The Device Layer (IoT / edge)
- Every REFILL+ Series 2 ships with **cellular connectivity built in** — no dependence on client WiFi. Aquablu states: "Every dispense streams to the AURA dashboard the moment it happens."
- The dispenser itself has digital surfaces: a **touchscreen UI** for drink selection (Aquablu employs a Senior Android Developer and is hiring an Android Engineer — strong signal the on-device UI runs on Android), plus embedded software (they employ Embedded & Full-Stack developers and are hiring an Embedded Software Engineer).
- Devices report telemetry continuously: dispenses (what, when, how much, at what temperature/carbonation), consumable levels (flavors, CO₂, filters), water quality, and system health.
- One tech-press description: AURA "operates through a network of interconnected nodes and monitors user preferences, consumption habits, and system status in real-time."

### Layer 2 — The Operations Layer (the B2B dashboard)
This is the facility manager / partner-facing side — the most documented part of AURA:
- **Real-time monitoring** of usage, system status, and performance across every unit in an organization (multi-location fleets in a single view).
- **Sustainability reporting:** live CO₂ savings and plastic-bottle-avoided counts per unit and per fleet — data companies use for ESG reporting. (Example: CMS Amsterdam's 7 dispensers have avoided 82,000+ bottles, with a tracked peak day of 147 liters on 19 March 2026 — the fact that Aquablu can quote a per-day, per-building liter count publicly is itself a demo of AURA's granularity.)
- **Proactive replenishment:** AURA "tracks every pour and flags refills before you run out." For BOLD, this goes further — "when flavors or boosts are nearly depleted, replacements are automatically shipped." Inventory management is automated end-to-end.
- **Predictive maintenance:** system flags filter changes and service needs before failures, "reducing costs and preventing downtime" — this feeds work orders to Aquablu's own Service Engineers.
- There is a live **partner portal at dashboard.aquablu.com** (behind sso.aquablu.com single sign-on) — evidence AURA is a real deployed web product, not vaporware.

### Layer 3 — The Personal Layer (the consumer experience, newest and fastest-moving)
Introduced with BOLD at CES 2026 — this is where AURA becomes an AI product:
- The **Aquablu app** connects to fitness trackers/wearables; a built-in **"hydration coach"** gives recommendations based on activity levels, hydration balance, and daily goals.
- **Tap-to-personalize:** "One tap of your phone is all it takes for the system to know exactly what you need" — the dispenser recognizes the user and adapts.
- **Learning loop:** AURA "learns from how and when someone drinks, adapts to taste preferences and lifestyle patterns." Marnix Stokvis's own demo line: *"After an intense workout, Aquablu BOLD recommends the Immunity variant with extra electrolytes and protein... The more I use it, the better it starts predicting my hydration need."* Users can flag preferences (e.g., lighter flavor) and the system persists them.
- **Location-level recommendation:** per their own description, "based on real hydration habits per location, we recommend the drinks that help people drink more, feel better, and build healthier routines."
- BOLD adds **integrated payment options** — meaning AURA also handles transactions in public/high-traffic deployments (gyms, hotels, airports).

---

## 3. The Data Flywheel (how to talk about AURA like a product person)

AURA's strategic value is a classic flywheel, and articulating it in an interview will set you apart:

1. **Every dispense is an event** → richest first-party dataset on workplace hydration behavior in existence (what flavor, what time, what temperature, which location, which machine).
2. **Data improves operations** → predictive restocking and maintenance keep uptime near-perfect and service costs low → Aquablu can promise "hydration-as-a-service" with a lean team (their stated goal: €100M revenue with <100 employees — only possible if AURA automates operations).
3. **Data improves the product** → the right flavors stocked per location, personalized recommendations, better hardware decisions.
4. **Data becomes the sales pitch** → facility managers get ESG numbers and usage insights they can show leadership; the Adyen "1.2 million bottles saved by 2030" forecast is an AURA-generated number used as marketing.
5. **Better experience → more usage → more data.** Repeat.

Marnix's positioning quote ties it together: hydration reframed "not as a commodity, but as infrastructure" — like coffee or internet service. AURA is what turns a water machine into infrastructure: measurable, controllable, justifiable to facilities, HR, and finance simultaneously.

---

## 4. AURA's Users & Stakeholders (map for product discovery talk)

| Persona | What AURA gives them | Their success metric |
|---|---|---|
| **End user / employee** | Touchscreen drink selection, app + hydration coach, wearable integration, personalized recommendations | Drinks more water, enjoys it, feels healthier |
| **Facility / office manager** | Fleet dashboard, auto-replenishment, maintenance alerts, ESG reports, zero admin | Uptime, zero complaints, sustainability numbers for leadership |
| **Client leadership (HR/finance/ESG)** | Quantified wellness benefit + plastic/CO₂ reporting | Justifiable spend, ESG targets |
| **Partners / resellers** (16 countries via channel) | Partner portal (dashboard.aquablu.com), multi-client fleet views | Service margin, client retention |
| **Aquablu internal — Service Engineers** | Predictive maintenance queue, remote diagnostics | Fewer truck rolls, faster fixes |
| **Aquablu internal — Logistics/Planning** | Consumption forecasts → automated shipment triggers | Stock efficiency, no stockouts |
| **Aquablu internal — Client Success** | Usage/adoption data per account | Retention, upsell |
| **Hotels / F&B managers** | Banquet beverage management, guest experience | Guest satisfaction, cost per serving |

Notice the job ad's phrasing — "the products our users hold, the platforms our clients and partners run on, and the tools our own crew works with every day" — maps exactly onto this table. A Digital Product Builder could own a slice anywhere in it.

---

## 5. Timeline of AURA

- **Pre-2025:** REFILL+ (Series 1) already connected and remotely monitored — the AURA capabilities existed in embryo ("hygienic, maintenance-free, connected system that is remotely monitored").
- **7 Oct 2025:** AURA formally launched and named, with REFILL+ Series 2. Rollout: Benelux, Germany, UK first; France + Scandinavia early 2026.
- **6 Jan 2026:** CES Las Vegas — BOLD launch positions AURA as an **"AI-driven hydration platform"**: wearable integration, hydration coach, auto-shipping consumables, payments. Aquablu explicitly brands itself as leading "AI-driven water technology."
- **2026:** AURA described as the umbrella platform for all products ("the AURA platform" listed alongside REFILL+ Series 2 and BOLD as one of three core products). Aug 2025 patent application on file (likely the cooling system, possibly platform-related).

## 1. What AURA Is (Aquablu's own words)

AURA is **"a platform that seamlessly connects Aquablu products and data in one intelligent system."** The page's tagline: **"easy. efficient. smart."** and **"one place for everything."**

In plain terms: AURA is the **single web platform** where a client (facility/office manager) or partner monitors and manages all their Aquablu dispensers, sees usage and sustainability data, and gets maintenance alerts. It's the software/data layer that sits on top of the physical REFILL+ and BOLD hardware.

**Important status signal:** the page's primary call-to-action is **"Let's talk"** linking to a **waitlist** (`/getintouch/waitlist-aura`). That tells you AURA — at least its newest/full form — is **still rolling out and not yet universally live to all clients.** This is a big deal for your business case: you're not building on a finished, mature platform; you'd be building on something Aquablu is actively standing up. (Framing tip: this makes "extend AURA into a new department" feel timely, not disruptive.)

---

## 2. The Four Pillars (straight from the page)

The product page organizes AURA around four capabilities. Learn these — they're the cleanest, most quotable summary of what AURA does:

1. **Power, made simple** — *"Monitor performance, usage, and remote access seamlessly."* Central monitoring and remote management of every system.
2. **Clarity at a glance** — *"See system health and customer behavior instantly."* Real-time health + behavioral view in one place.
3. **Trends that matter** — *"See flavor usage and preferences to fuel growth."* Consumption/flavor analytics framed explicitly as a **growth** lever, not just ops.
4. **Track your impact** — *"Monitor CO₂ and plastic bottle reduction in real time."* Live sustainability/ESG reporting.

Two supporting themes the page repeats:
- **"Centralized power. Faster moves."** — *"Manage all REFILL+ hydration systems from one place and receive timely cleaning and maintenance alerts."*
- **"Powerful insights. Made to scale."** — *"Get data-powered insights that help you predict, act with precision and make smarter decisions."* (Note the word **predict** — AURA is positioned as predictive, not just descriptive.)

---

## 3. How You Access It (concrete, verified)

- **One login / Single Sign-On (SSO).** The page states: *"Access all tools with Single Sign-On and an intuitive interface."* AURA is explicitly a **suite of tools behind one SSO** — "one login, effortless control."
- **Partner portal** lives at **`dashboard.aquablu.com`** / **`sso.aquablu.com/login`** — the real, deployed entry point (this is the operations/partner side).
- **Client login / shop** runs through a separate **Shopify-backed** store auth (`store.aquablu.com`) — so consumables/reordering commerce is on Shopify, distinct from the AURA operational dashboard. *(Useful architectural tell: commerce = Shopify; operations/monitoring = AURA dashboard. Two different systems a CSM might touch.)*
- **Multi-site by design.** The FAQ explicitly addresses *"managing multiple systems across different offices,"* confirming AURA handles fleets across locations under one account — relevant for enterprise clients like CMS (7 units) or Adyen.

---

## 4. What AURA Connects To (the hardware underneath)

- **REFILL+ Series 2** — ships with **built-in cellular connectivity**; every dispense streams to AURA in real time (from the Series 2 launch). AURA is described as its management brain.
- **BOLD** (CES 2026) — also AURA-powered; adds **automated inventory management** (auto-ships flavors/boosts when low) and the **consumer-facing** personalization layer (app, hydration coach, wearable integration).
- The Service Terms give AURA contractual weight: the **Aquablu Dashboard is written in as "binding evidence"** of whether a client performed required sanitation. So AURA isn't just a convenience layer — it has **legal standing** in the client relationship.

---

## 5. The Five FAQ Topics (what clients ask — and what to expect AURA does)

The page's FAQ headings map the client-facing scope:
1. **What is AURA and how does it work with all REFILL+ systems?** — the umbrella/connector question.
2. **How does AURA help with maintenance and performance optimization?** — predictive maintenance + cleaning/service alerts.
3. **Can AURA track sustainability impact?** — yes; CO₂ + bottles saved, real-time.
4. **Is AURA suitable for managing multiple systems across different offices?** — yes; multi-site fleet management.
5. **How do I access AURA and what does the setup look like?** — SSO + onboarding/setup.

These five are effectively AURA's official value pillars restated as client questions — a clean checklist of what the platform promises.

---

## 6. Why AURA Matters for Your Business Case (the CS/Aura brief)

Your case is literally about extending **Aura** into Customer Success. This page sharpens several arguments:

1. **AURA is already "one place for everything" — for clients.** The brief's vision ("one platform where everyone at the company works") is AURA's *own marketing promise* turned inward. You're proposing to do for CS internally what AURA already does for facility managers externally. That's a *consistent extension of the product's stated philosophy*, not a new idea imposed on it — a strong framing.
2. **SSO + "suite of tools behind one login" is the existing pattern.** AURA is already architected as multiple tools under one SSO. Adding a CS workspace is architecturally *native* to how AURA is built — not a bolt-on. Say this.
3. **The data CS needs is already flowing in.** "Monitor performance, usage… see system health and customer behavior instantly… predict." AURA already ingests exactly the usage/health signals a CS health-score view would need. Your wedge (join usage + account context) is mostly a *surfacing/join* problem, not a *capture* problem.
4. **"Trends that matter… to fuel growth."** AURA already frames consumption data as a growth/commercial lever — which is the bridge to CS's retention/upsell mandate. You're not repurposing an ops tool; you're extending a tool that's *already* pointed at growth.
5. **It's still being rolled out (waitlist).** You'd be building alongside an actively-growing platform, with a digital team (Thijmen – Senior PM Digital, Miriam – UI/UX, Mees, Alessandro) plus Data/AI folks (Artjoms – Data Analytics Lead, Thomas – Automation & AI, Dylan – AI Solutions). Smart to acknowledge you'd build *with* them and inherit AURA's existing SSO, design system, and data model rather than reinvent.
6. **Honest gap to probe:** the public page is deliberately high-level — it does **not** reveal the tech stack, what data AURA exposes via API to internal teams, or how much of "predict" is live ML vs. roadmap. Those are exactly the questions to ask in the specialist round ("How much of AURA's data is accessible to internal tools today? Is the 'predict' capability live or planned?").

---

## 7. Quick-Reference Card

| | |
|---|---|
| **Official line** | "A platform that seamlessly connects Aquablu products and data in one intelligent system." |
| **Tagline** | "easy. efficient. smart." / "one place for everything" |
| **Four pillars** | Power made simple (monitor/usage/remote) · Clarity at a glance (health + behavior) · Trends that matter (flavor analytics for growth) · Track your impact (CO₂ + bottles, real-time) |
| **Access** | Single Sign-On; suite of tools behind one login; intuitive UI |
| **Portal** | dashboard.aquablu.com / sso.aquablu.com (partner/ops); Shopify-based client shop for commerce |
| **Multi-site** | Yes — manage multiple systems across offices from one account |
| **Positioning** | Predictive ("predict, act with precision"), scalable, growth-oriented |
| **Connects** | REFILL+ Series 2 (cellular, live dispense streaming), BOLD (auto-restock + consumer app) |
| **Contractual weight** | Aquablu Dashboard = "binding evidence" of sanitation compliance (Service Terms) |
| **Status** | Actively rolling out — page CTA is a **waitlist**, not "log in" |
| **Case relevance** | The brief's "one platform for everyone" = AURA's own promise, turned inward toward CS |

---

*Sources: aquablu.com/products/aura (official product page — pillars, SSO, waitlist, FAQ, taglines), aquablu.com Series 2 launch & /products/refill-series-2 (cellular streaming), aquablu.com/stories/bold + CES 2026 press release (BOLD/auto-restock/consumer layer), aquablu.com/service-terms (Dashboard as binding evidence). Compiled August 2026. The product page is intentionally high-level marketing; internal architecture, APIs, data-access model, and the live-vs-roadmap status of predictive features are not public and should be treated as questions for the specialist round.*
