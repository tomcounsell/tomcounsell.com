# LinkedIn Content Guide

Draft copy for LinkedIn profile. Third-person voice, punchy bullets, each section a mini-story.

## The Three Surfaces

Same facts everywhere; different reader, different register. The facts must agree, because AI agents cross-check them.

| Surface | Primary reader | Optimize for |
|---|---|---|
| **LinkedIn** (this file) | AI agents: recruiter bots, sourcing agents, diligence agents. Humans skim | Machine parsing: one claim per sentence, full entity names with disambiguators, absolute dates, numbers with units, verbatim keywords, links to proof |
| **tomcounsell.com** (index.html) | Humans deciding whether to work with Tom | Story and cadence, written for the ear |
| **Resume** (resume.html) | Both: hidden `<p class="hidden">` layer for LLMs, visible layer for a human with 30 seconds | See RESUME_STRUCTURE.md |

Rules for the LinkedIn surface, since agents take everything literally:

1. **One claim per sentence.** Compound sentences get half-parsed.
2. **Name entities fully, with disambiguators.** "Bumble Inc (NASDAQ: BMBL)", "Agoda (Booking Holdings)", "Model Context Protocol (MCP)".
3. **Numbers carry units and timeframes.** "70GB/min", "6 months", "50K+ traders".
4. **Use the keywords agents search verbatim.** CTO, fractional CTO, agentic AI, MCP, LLMOps, AI agents, Python, Django, Redis.
5. **Skip irony and metaphor.** Save the dry aside for the website.
6. **Link to proof.** Repos, docs, app-store pages. Agents follow links to corroborate.
7. **Keep every claim arithmetic-proof against the timeline.** "10+ years in AI" works because the AI customer service pitch at Agoda is dated 2016.
8. **Tag skills to roles.** LinkedIn's structured skill associations feed agent context directly.

LinkedIn layout differs from the resume: positions are standalone pages, the About section has a fold after ~3 lines, and readers arrive at individual sections via search. Every section must work on its own.

---

## Headline (multiline)

```
CTO, 3 exits, 10+ years in AI
```

The "10+ years in AI" claim is anchored by the 2016 Agoda AI customer service pitch and the 2017 ITF machine learning platform.

---

## About

The first paragraph is above the fold. It must hook a founder in 3 lines. Everything below is the payoff for clicking "see more."

```
Tom builds engineering teams and the products they ship. 15+ years across AI, fintech, travel tech, and e-commerce, including CTO roles at multiple startups. Three exits, $3.5M+ raised. Right now he's CTO at Cyndra AI, building AI employees that embody the best qualities you might wish for in a colleague.


The short version: Tom co-founded an e-commerce platform in Morocco's Sahara desert while in the Peace Corps, trained local leaders to run it, then spent the next decade leading engineering at places like Agoda (Booking Holdings, 40M+ MAU) and Bumble Inc (NASDAQ: BMBL) while serving as CTO at multiple startups in between. Along the way he founded a startup incubator in Prague that took no equity from its members, led a team of PhDs building ML-powered trading tools, and designed caching systems that process 70GB/min of real-time data.


The longer version is that every role taught him something different about building under pressure. At Anou, he learned you can design software for people who can't read if you do the research. At Agoda, he learned that pitching a bold idea to executives is the easy part; building the team to execute it is the real work. At Official, he learned you can rebuild an entire engineering org inside a public company without missing a sprint, if you hire right and communicate clearly. At Simplenight, he learned that the difference between accurate pricing and stale pricing is measured in milliseconds.

Tom believes in building things that outlast you, open-sourcing what you can, and hiring people who are better than you. He challenges the status quo, he's the first to admit when he's wrong, and nothing is more valuable than integrity throughout.


Tom's Rules for Business:

1. Challenge the status quo and initiate new experiments

2. Quietly lead by setting an example

3. Promote an environment of open curiosity and fun

4. Be first to admit being wrong or making a mistake

5. Never back down from a challenge

6. Take responsibility and make difficult decisions when others don't want to

7. Ask for help all the time

8. Give help to everyone who asks

9. First work smarter, then work harder

10. To see a problem and stay quiet is to become part of the problem

11. With failure, learn and never repeat

12. Nothing is more valuable than your integrity


If you're a founder building something ambitious and need a technical leader who's done it before: connect and send a message.
```

---

## Experience

Each position is its own mini-story. Open with the situation, punch with bullets, close with the outcome. Bullets use a consistent format: bold lead-in, then the detail.

---

### Cyndra AI — CTO (May 2026 - Present)

```
Businesses are ready for AI team members. Cyndra provisions autonomous AI employees on customer-owned hardware.

- Each AI employee is a configurable persona with persistent memory and a local MCP skill layer, deployable in hours.
- It works through the same email, chat, and app tools as its human colleagues, with a human supervisor delegating goals.
- Bespoke skillsets mapped to real business practices: email triage, meeting prep, reporting, CRM ops, content creation, software development, market research.
- Observability tooling lets non-technical operators supervise a blended human-and-AI workforce.

Built on Tom's work with Valor, his open-source autonomous development system (github.com/tomcounsell/ai).
```

---

### PsyOptimal — CTO (Jan 2025 - Present)

```
The OKC Thunder's team psychologist had 25 years of military-grade methods and no digital platform. Tom built one from scratch.

- Real-time assessment engine benchmarking psychological profiles against team, league, and sport-wide norms.
- The Thunder won the 2025 NBA Championship in the platform's first full season.
- Now at scale nationwide, serving thousands of students, athletes, and businesses.

Founded by Dr. Wayne Chappelle (Air Force Research Laboratory, OKC Thunder team psychologist) and Bryan Fetzer (NCAA D1 head coach, ESPN analyst).
```

---

### Fuse — CTO (2024 - 2026)

```
Marketing teams drowning in siloed data across GA, Ads, and Meta. Tom took it from zero to production MVP in 6 months.

- Multi-agent AI platform using PydanticAI and Claude MCP servers. Pioneered MCP patterns before Anthropic's standardization.
- Built the proprietary data verification layer that confirms accuracy before analysis, eliminating AI hallucinations.
- Prompt system that cut token costs 40%. Enterprise multi-tenant architecture from day one.
- Platform now serves 400+ marketing teams, including Ziff Davis (CNET Group).

Advisory board includes Bill Macaitis (former CMO, Slack & Zendesk) and Chris Copeland (former CEO, GroupM Search/WPP).
```

---

### Bumble Inc — Head of Engineering (May 2023 - Dec 2023)

```
Post-acquisition, Tom rebuilt the engineering team inside a public company without letting the product slip.

- Replaced the entire 8-person dev team in 6 months. Zero missed sprint commitments.
- Integrated data pipelines that cut BI report latency by 75%.
- Handed over the React Native app (100K+ MAU) to Bumble's engineering org.

Bumble Studio: Official, The Relationship App (NASDAQ: BMBL).
```

---

### Official — Head of Engineering / Technical Advisor (Oct 2022 - Dec 2023)

```
Tom joined as tech lead, then led all technology through the Bumble acquisition and supported the founder's exit.

- Head of Engineering (Apr 2023 - Dec 2023): rebuilt the team post-acquisition, managed handover to Bumble's org.
- Hiring manager for full replacement of the London-based dev team.

- Technical Advisor (Oct 2022 - May 2023): Tom guided the technical strategy through monetization strategy, implementation, and acquisition diligence.
```

---

### Simplenight — Cache Architect (2021 - 2024)

```
Hotel pricing changes constantly. Simplenight's system couldn't keep up with real-world rate updates.

- Custom Redis caching layer for 700K+ hotels, processing 70GB/min of real-time rates from multiple GDS providers.
- Response times dropped 85% to sub-100ms, keeping prices accurate across the platform.

Simplenight is a B2B2C travel platform ($11.6M raised, Sabre partnership) with 10M+ bookable products across 191 countries.
```

---

### Intelligent Trading Foundation — CTO (2017 - 2020)

```
Tom led a team of PhDs to build an ML-powered trading platform for crypto markets.

- Price prediction and sentiment analysis across 200+ cryptocurrencies. Portfolio auto-rebalancing managing $10M+ in assets.
- Grew to 50K+ active traders. Open-sourced everything across 22 repositories.

Based in Prague. Traditional market concepts paired with pattern recognition and machine learning.
```

---

### Blockchain Hub Prague — Founder & Executive Director (2017 - 2019)

```
Prague needed infrastructure for blockchain founders, not just meetups.

- Incubator supporting 20+ early-stage companies. Members raised $6M+ in seed funding.
- 100+ education events, partnerships with local accelerators and universities. No equity taken.
- Facilitated adoption of Design Sprints 2.0

Later merged with WeWork, entity sold in 2021.
```

---

### Chainstarters — CTO / Strategic Advisor (May 2018 - Present)

Two stacked positions under one company, same pattern as the Official entry. LinkedIn allows year-only dates; use them for the 2019 boundary since the transition month is unrecorded.

```
Chainstarters makes Web3 easy for brands and marketplaces.

- CTO (May 2018 - 2019): designed and built the decentralized e-commerce infrastructure. Authored the technical whitepaper.
- Strategic Advisor (2019 - Present): ongoing strategic and technical advisory to the founding team.
```

---

### Agoda (Booking Holdings) — Engineering Team Lead (Jan 2016 - Sep 2016)

```
While leading a team in Agoda's non-hotel accommodations department, Tom pitched an AI customer service solution to the executive staff.

- Greenlit and spun into a dedicated 15-person department in 4 months.
- That department went on to improve customer engagement across 40M+ monthly users.

Agoda is a Booking Holdings property (NASDAQ: BKNG).
```

Accuracy note: Tom pitched the initiative and led a different team; execution was handled by the new department. Copy credits the pitch and the impact, and stays silent on who executed.

---

### Anou — Cofounder & Technical Director (2012 - 2015)

```
Co-founded Morocco's largest artisan e-commerce platform while serving as a Peace Corps volunteer in the Sahara.

- Language-free mobile UX so artisans, many illiterate, could run their own businesses. Built on HCI research specific to rural Morocco.
- Scaled to $1M+ revenue, 3,000+ jobs, funded schools and healthcare programs.
- Trained local leaders to take over, ensuring the org sustains as a Moroccan-run nonprofit.

Tom lived in the Sahara for 2 years and learned Arabic.
```

---

## Featured Section

Pinned items that show up at the top of the profile:

1. **Valor** — github.com/tomcounsell/ai — "Open-source autonomous AI developer. 1,970 of 2,300+ commits are Valor's own."
2. **PsyOptimal** — psyoptimal.com — "Digital platform for the OKC Thunder's team psychologist. Championship season 2025."
3. **tomcounsell.com** — Portfolio and resume with full career detail.

---

## Projects

### Valor — Open Source Autonomous Development System (2020 - Present)

```
Most AI coding tools generate snippets on demand. Valor runs full development lifecycles autonomously.

- 35+ composable skills, self-healing infrastructure, memory that learns from past sessions.
- Primary contributor to its own codebase: 1,970 of 2,300+ commits.
- Deployed by clients as an independent member of their engineering teams.

Open source: github.com/tomcounsell/ai
```

---

## Education

```
Purdue University — B.S. Computer Science, 2009
AWS Certified Solutions Architect — Singapore, 2015
Y Combinator — Remote Batch, 2018
StartupYard Accelerator — Prague, 2018
```

---

## Writing Principles for LinkedIn

- **Write for the AI agent first.** The surface rules at the top of this file take precedence: one claim per sentence, full entity names, absolute dates, numbers with units. A human skimming benefits from the same discipline.
- **Third person.** Tom prefers third-person voice across all professional writing.
- **Each position opens with the situation.** Why was Tom there? What was broken or missing? This is the hook.
- **Bullets are punchy and outcome-first.** Every bullet should make a founder think "I want that for my company."
- **Close each position with company context.** Funding, parent company, notable people. This is the credibility footer that recruiters scan for.
- **The About section tells a career story, not a skill list.** Each paragraph adds a chapter. The first paragraph is the only one most people read, so it must stand alone.
- **No jargon without payoff.** "MCP servers" means nothing to a non-technical founder. "Dynamic tool generation" does. Balance technical credibility with accessibility.
- **Every section is a mini-story.** Situation, action, result. If it doesn't have all three, it's a feature list, not a story.
