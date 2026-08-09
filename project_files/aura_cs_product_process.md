# Product Process: Bringing Customer Success into Aura


---

## Phase 0 — Business Strategy Alignment (anchor everything in where Aquablu is going)

**Goal:** Before looking at CS workflows, understand the company-level goals that should determine which CS problems are worth solving first. The workflow you choose to build isn't just the most painful one — it's the one that best serves where Aquablu is headed.

### Aquablu's strategic context (2025–2028)

**Growth trajectory:**
- 300% year-over-year growth for three consecutive years
- Reached profitability for the first time in April 2025
- Raised €7M seed round led by Frans van Houten (former Philips CEO)
- Target: €100M revenue by 2028 with fewer than 100 employees (~88 today)

**Expansion:**
- Currently operating in 16+ European countries (Benelux, Germany, UK)
- Expanding into 10+ additional European countries in 2026
- US market debut at CES 2026 with Aquablu BOLD
- Enterprise clients include Heineken, Adyen, Microsoft — serving 100,000+ daily users

**Product portfolio is splitting:**
- REFILL+ Series 2: Built-in workplace system for offices and hotels (25+ employees), powered by AURA
- Aquablu BOLD: Standalone, plug-and-play dispenser for gyms, airports, hotels, public spaces — broader market, more locations, different customer profile

**Platform vision (from the brief):**
- AURA started as a machine dashboard (telemetry, service state, account data)
- Now being extended into "the place where Aquablu itself runs" — the internal operating layer
- Currently provides: real-time usage insights, CO₂/plastic savings reporting, system performance monitoring, automated supply management

**Aquablu Company top objective:**
- Maximize ARR

### What this means for CS workflow prioritization

These business goals create specific filters for what to build:

| Business goal | CS implication | Prioritization filter |
|---|---|---|
| €100M with <100 people | CS must scale without headcount. Every workflow you build should reduce manual effort per account. | Favor automation-heavy workflows over ones that just reorganize manual work |
| 10+ new countries in 2026 | CS will onboard customers in markets where Aquablu has no local presence. Remote onboarding and monitoring become critical. | Favor workflows that work across geographies without requiring in-person interaction |
| Two product lines (REFILL+ and BOLD) | CS now manages two different customer profiles with different needs. BOLD customers (gyms, airports) are higher volume, lower touch. | The workflow should handle both product lines, or you should be explicit about which one you're solving for and why |
| 300% YoY growth | The installed base of machines is growing fast. Reactive support doesn't scale. | Favor proactive workflows (health monitoring, usage-based outreach) over reactive ones (ticket handling) |
| AURA as the internal operating layer | This isn't just a CS tool — it's the first department migration. The pattern you set will be replicated. | The workflow should demonstrate that Aura can replace external SaaS, not just supplement it |
| Data already in AURA | Telemetry, service state, usage, CO₂/plastic savings, system performance are already there. | Build on existing data. Don't start with workflows that require integrating new data sources from scratch |

### The strategic question to answer before proceeding

"Which CS workflow, if moved into Aura, would most directly enable Aquablu to maximize ARR and manage more accounts with the same team size — across multiple countries and both product lines?"

That's the business case. Everything downstream should ladder up to it.

---

## Phase 1 — Discovery (understand the world before touching the product)

**Goal:** Build a mental model of how Customer Success actually works today — not how anyone thinks it should work.

**What to do:**

Map the CS department across three layers:

- **People.** Who is on the team? What are their roles (onboarding specialist, account manager, support, renewals)? Who do they interact with outside CS (sales handoff, field service, finance)?
- **Jobs.** What does each person actually do in a day? Not their job description — their real routines. What decisions do they make, what information do they need to make them, and where does that information live?
- **Tools.** Which SaaS products does CS currently touch(different software platforms like an ERP, a CRM, a planning tool for maintenance and an online store)? For each tool, what data lives there, what actions happen there, and what's the handoff to the next tool?

**Key questions to answer:**

- What is the single task a CS person does most often?
- Where do they waste the most time — context-switching, searching for data, copying information between tools, waiting for someone else?
- What information from Aura's existing telemetry/service data would change how they do their job if they had it at hand?
- What breaks? Where do things fall through the cracks between tools?

**Methods (given the constraint):**

Since you have limited access, work with what you can infer and validate. Aquablu makes water dispensing systems. Aura already holds telemetry, service state, and account data. CS in a hardware/IoT company like this typically covers: onboarding new accounts after install, monitoring machine health proactively, handling support issues, managing service contracts/renewals, and tracking customer satisfaction. Cross-reference this with the brief's statement that "a single task routinely spans four tools."

**Output:** A one-page map — the CS workflow landscape. People, their jobs, the tools they use, and the pain points between them.

---

## Phase 2 — Problem framing (decide what to attack)

**Goal:** Pick one specific, high-impact workflow to migrate into Aura. Not the whole department — one workflow.

**Prioritization framework — score each candidate workflow on:**

| Criterion | What it means |
|---|---|
| **Pain severity** | How much friction does the current process cause? (time wasted, errors, things falling through cracks) |
| **Frequency** | How often does this workflow happen? (daily > weekly > monthly) |
| **Data proximity** | How much of the data this workflow needs is already in Aura? (telemetry, service state, account data) |
| **Cross-tool span** | How many external tools does this workflow currently touch? (more = more context-switching = more value in consolidating) |
| **Downstream value** | Does solving this unlock value for other departments or workflows? |
| **Buildability** | Can you build a meaningful v1 in the time you have? |

**The sweet spot:** A workflow that is high-frequency, high-pain, and already data-adjacent to what Aura holds. For an IoT water dispenser company, the most likely candidates are:

**Decision criteria for the case:** Pick the workflow where Aura's existing data (telemetry, service state, account info) is most central. That's your unfair advantage — the data is already there, you're building the workflow layer on top of it.

**Output:** A problem statement in the format: *"[CS role] needs to [do what] when [trigger], but today this requires [current painful process across N tools], which causes [specific negative outcome]."*

---

## Phase 3 — Define outcomes (what does "working in Aura" look like?)

**Goal:** Describe the future state — not features, but outcomes. What changes for the CS team when this workflow lives in Aura?

**Outcome levels:**

**User outcome (the CS person):**
- What can they do that they couldn't before?
- What takes less time?
- What information do they no longer have to hunt for?
- What decisions can they now make faster or better?

**Business outcome (Aquablu):**
- Does this reduce churn? By catching issues earlier?
- Does this increase response time to customer issues?
- Does this reduce the number of tools the company pays for?
- Does this make CS knowledge less dependent on individual people?

**Platform outcome (Aura):**
- Does this create a reason for CS to open Aura daily? (habit formation = adoption)
- Does this generate new data that makes Aura more valuable? (e.g., customer interaction logs alongside machine telemetry)
- Does this establish a pattern that other departments can follow?

**Output:** 3–5 outcome statements, each tied to a level. Example: *"A CS manager can see which accounts have machines showing degraded performance and reach out before the customer reports an issue — without leaving Aura."*

---

## Phase 4 — Define KPIs (how you'll know it's working)

**Goal:** Set measurable indicators that connect back to the outcomes. Not vanity metrics — signals that tell you whether the workflow migration is actually solving the problem.

**KPI categories:**

**Adoption KPIs (is CS actually using it?):**
- Daily active users in the CS workflow (target: 100% of CS team within 4 weeks)
- Sessions per user per day
- Time spent in Aura vs. time spent in the tool it replaced
- Drop-off rate (do they start in Aura but finish the task elsewhere?)

**Efficiency KPIs (is it faster/better?):**
- Time-to-resolution for the target workflow (before vs. after)
- Number of tool switches per task (target: zero — the whole workflow completes in Aura)
- Manual data entry eliminated (e.g., no longer copying machine IDs between systems)

**Quality KPIs (is the work output better?):**
- Issues caught proactively vs. reactively (if the workflow is health monitoring)
- Customer response time
- Tasks that fell through the cracks (missed follow-ups, forgotten renewals)

**Business KPIs (does it move the needle?):**
- Customer churn rate (lagging indicator, but the north star)
- NPS or CSAT scores
- Revenue retained through successful renewals
- Reduction in external SaaS spend

**Setting targets:** For a v1, focus on adoption and efficiency. You can't move business KPIs with a first build, but you can prove the workflow is faster and people are using it. That earns the right to keep building.

**Output:** A KPI dashboard spec — 6–8 metrics with current baseline (even if estimated), target, and measurement method.

---

## Phase 5 — Solution design (now you can talk about what to build)

**Goal:** Design the minimum product that delivers the target outcome for the chosen workflow.

**Design principles for this case:**

- **Data-first, not feature-first.** The most valuable thing Aura can do is surface the right information at the right time. Before adding any workflow capability, make sure the data layer is right — the CS person sees what they need without searching.
- **Replace a tool, not a task.** Don't build "a little CRM inside Aura." Build the specific workflow that currently lives across multiple tools, and make it complete enough that the CS person never needs to leave Aura for that workflow.
- **One workflow, done fully.** It's better to handle one workflow end-to-end than to partially cover three. Partial coverage means the person still has to use the old tools anyway, which means they won't switch.
- **Use Aura's existing strengths.** Telemetry and machine data are already there. Build on top of that unique asset rather than rebuilding generic CRM features.

**What a v1 should include:**

1. A view — what does the CS person see when they open this workflow? (the information architecture)
2. A trigger — what kicks off the workflow? (an alert, a schedule, a manual action)
3. An action path — what does the CS person do, step by step, to complete the workflow inside Aura?
4. A completion state — how does the system know the workflow is done? What gets recorded?

**Output:** A lightweight spec: user story, screen-by-screen flow, and data requirements. Then build it.

---

## Phase 5b — Assumptions & Risk Log

**Goal:** Make explicit what you're betting on, so you can validate or kill assumptions early.

Every product decision rests on assumptions. Logging them isn't bureaucracy — it's how you avoid building something nobody uses because you never questioned your own premise.

**Assumption categories:**

**User assumptions:**
- "CS actually context-switches between 4+ tools for this workflow" — Validate by observing, not asking. People undercount or overcount tool switches.
- "The data in Aura is sufficient for this workflow" — Check what's actually there vs. what you think is there. Telemetry might not include the fields CS needs.
- "CS will prefer doing this in Aura over their current tool" — The current tool might have features or muscle memory you're underestimating.

**Business assumptions:**
- "This workflow is the highest-leverage one for scaling" — You're choosing based on research, not data. Flag that the ranking could be wrong.
- "The pattern from CS can be replicated for other departments" — The next department might have fundamentally different needs.

**Technical assumptions:**
- "Aura's existing data model supports the workflow without major backend changes" — Verify early.
- "Aura can handle the UX requirements of a workflow tool, not just a dashboard" — A dashboard and a workflow engine are architecturally different.

**Risk log format:**

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| CS team doesn't adopt because existing tools are "good enough" | Medium | High | Build around a workflow that genuinely can't be done well in existing tools (e.g., machine telemetry + customer action in one view) |
| Data in Aura is incomplete for the chosen workflow | Medium | High | Audit Aura's actual data schema before designing the UI |
| Building for REFILL+ but BOLD grows faster, making the workflow irrelevant | Low | Medium | Design workflow patterns that are product-agnostic where possible |
| First department migration sets wrong architectural precedent | Low | High | Document the pattern explicitly so it can be evaluated before replicating |

---

## Phase 6 — Build, validate, iterate

**Goal:** Ship the v1, learn whether the outcomes are being achieved, and decide what to do next.

**For the case exercise:** You're building a working prototype. Fake data is fine. The point is to demonstrate that the workflow is coherent — that a CS person could sit down, open Aura, and complete the target task without leaving.

**Validation plan (post-prototype, for the real product):**

- **Week 1:** Put it in front of 2–3 CS team members. Watch them use it. Note where they get stuck, where they revert to old tools, where they say "but I also need..."
- **Week 2–4:** Soft launch with the full CS team. Track adoption KPIs daily. Hold a weekly feedback session.
- **Month 2:** Evaluate efficiency KPIs. Is the workflow actually faster? Are tool switches eliminated?
- **Month 3:** Decide whether to deepen this workflow or start the next one.

**Iteration logic:**

- If adoption is low → the workflow doesn't match their real routine (go back to Discovery)
- If adoption is high but efficiency hasn't improved → the UI or data is wrong (iterate on Solution Design)
- If both are high → start Phase 2 again for the next workflow

---

## Phase 7 — Change Management & Adoption (the phase most internal tools skip)

**Goal:** Make sure CS actually switches. The best workflow in the world fails if nobody uses it.

This is especially critical at Aquablu because the brief says the company "runs on a patchwork of external SaaS." People have habits. They know where things are. Asking them to move to Aura isn't just a feature question — it's a behavior change question.

**Why internal tools fail at adoption:**

1. The tool covers 80% of the workflow, so people still need the old tool for the remaining 20% — and once they're in the old tool, they do everything there.
2. The tool is built for how management wants people to work, not how people actually work.
3. There's no forcing function. Nobody turned off the old tool.
4. No one explained *why* this matters to *them* — only why it matters to the company.

**Adoption strategy for Aura CS workflows:**

**Before launch:**
- Identify 1–2 CS power users as design partners. They co-create the workflow, which makes them advocates.
- Be transparent about what Aura replaces and what it doesn't (yet). Partial honesty breeds more distrust than full honesty.
- Set a date for when the old tool access goes away. Without this, adoption is optional, and optional means never.

**At launch:**
- Make the first experience a "wow" moment — something Aura can do that the old tool literally cannot. For Aquablu, this is likely: machine telemetry + customer context in one view. No CRM shows you filter pressure alongside the account record.
- Provide escape hatches for edge cases, but log every time someone uses them. That's your roadmap for v2.

**After launch:**
- Track the "last tool standing" — which external SaaS tool is the last one CS still opens? That tells you what to build next.
- Celebrate milestones publicly: "CS closed 50 proactive outreach tasks this week without leaving Aura."

**Metrics for adoption specifically:**
- Percentage of target workflow completions happening in Aura vs. old tools (target: 100% within 6 weeks)
- Number of times CS opens the old tool for the target workflow (target: zero)
- CS team satisfaction score with Aura (survey at week 2 and week 6)

---

## How this maps to the 4-hour constraint

| Time | Phase | Output |
|---|---|---|
| 0:00–0:30 | Phase 0: Business Strategy Alignment | Strategy summary, prioritization filters |
| 0:30–1:00 | Phase 1–2: Discovery + Problem Framing | CS workflow map, chosen workflow, problem statement |
| 1:00–1:20 | Phase 3–4: Outcomes + KPIs | Outcome statements, KPI list |
| 1:20–1:30 | Phase 5b: Assumptions & Risks | Logged assumptions, top risks |
| 1:30–3:15 | Phase 5: Solution Design + Build | Working prototype |
| 3:15–4:00 | Presentation prep | 15-minute narrative tying strategy → process → product |

Phases 6 and 7 (Validate and Change Management) are post-build — you present them as your plan for what happens after shipping, not as something you execute during the 4 hours.

**Presentation structure (15 minutes):**

1. (~2 min) "Here's where Aquablu is going" — the business context and why it matters for what CS needs
2. (~2 min) "Here's what I learned about CS" — the workflow landscape and pain points
3. (~2 min) "Here's the problem I chose and why" — the prioritization logic, tied back to business goals
4. (~2 min) "Here's what success looks like" — outcomes and KPIs
5. (~5 min) "Here's what I built" — live demo of the prototype
6. (~2 min) "Here's what happens next" — validation plan, adoption strategy, and the path to the next department

This structure shows strategic product thinking, not just design or engineering skill. It proves you can connect a company's business trajectory to a specific workflow decision to a working product.

---

## The meta-argument

The brief says: *"figuring that out is the job, and how you go about it is what we're actually interested in."*

This process is your answer to "how you go about it." Starting with Aquablu's business goals (Phase 0) proves you're not solving CS pain in a vacuum — you're solving the CS pain that most directly enables €100M revenue with <100 people across 26+ countries. The prototype is evidence that the process produces something real. The presentation is the story that connects strategy to product.

The strongest signal you can send is: "I understand where your company is going. I have a method for turning that direction into specific product decisions. And I can ship."
