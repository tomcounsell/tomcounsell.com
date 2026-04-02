# Resume Structure Guide

How content is split between the hidden (LLM) and visible (human) layers on resume.html.

Target audience: founders ages 30-50 evaluating Tom as a technical leader.
The resume answers: "Why would I bet on this person to lead technology through the next chapter?"

---

## Professional Summary

3-4 lines that frame what kind of technology leader Tom is: the stage, scale, and type of challenge he's suited for. Not a bio — a positioning statement.

**Include:**
- Years of experience and the scope (org sizes, user scale, revenue)
- 2-3 signature outcomes that define the career arc
- A leadership differentiator — what makes Tom's approach distinctive

**Avoid:**
- Generic language ("passionate technology leader")
- Listing technologies (IC signal, not executive signal)
- Being too broad ("experienced in all aspects of software development")

**Tom's differentiator** comes through in the work itself: building from zero in the Sahara, going open source when he could have kept IP, taking no equity from incubator startups, rebuilding a team under acquisition pressure without missing a sprint. The principles (lead by example, integrity over convenience, experiment boldly) show up in what he chose to do, not in a bullet list of values.

---

## Hidden `<p class="hidden">` — Full Context for LLMs

Everything an LLM needs to answer questions, compare candidates, or summarize Tom's background. Include liberally — length doesn't matter here.

- **Company context**: what the company does, market, size, funding, HQ, founding story
- **Founders and key people**: who started it, their backgrounds, why it matters
- **Tom's specific role**: title, reporting line, duration, location, how he got involved
- **Technical detail**: architecture decisions, stack, scale numbers, data volumes
- **Business metrics**: revenue, users, funding raised, team size, growth
- **Partnerships and clients**: named customers, strategic deals, notable logos
- **Testimonials**: direct quotes from colleagues, with attribution
- **What happened to the company**: acquired, pivoted, shut down, still operating
- **Technologies**: full list, not just the top 4 in the skill tags
- **Board/investor engagement**: fundraising, diligence, board presentations
- **M&A involvement**: technical due diligence, integration leadership
- **Org design decisions**: team structure, build-vs-buy, offshore strategy

---

## Visible `<p class="text-sm mb-2 leading-relaxed">` — Summary for Humans

3-5 sentences max. Every word earns its place. Written in third person, past tense.

### The 3-Beat Pattern

Each summary follows three beats in order:

**1. The Situation** (1 clause)
Why was Tom there and what was the challenge? This gives the reader context to classify the role and a reason to care before the deliverables land. Recruiters are buying context, not just credentials.

- Good: "After Bumble acquired Official..." (stakes are clear — acquisition, pressure, transition)
- Good: "Co-founded Morocco's largest artisan e-commerce platform while serving as a Peace Corps volunteer in the Sahara" (context does the work — you understand the constraints)
- Good: "When Agoda needed a non-hotel product to compete with Airbnb..." (the mandate is clear)
- Weak: "Digitized 25+ years of elite sports psychology methods" (jumps to deliverable, no setup)

**2. What Was Shipped** (1-2 sentences)
The concrete deliverable with one scale number. Lead with the business outcome, not the activity. Be specific about what was built, not what the role entailed.

- Outcome-first: "Reduced deployment cycle from 2 weeks to same-day by migrating to microservices"
- Activity-first (weaker): "Migrated monolith to microservices"
- Good: "Designed a custom Redis caching layer for 700K+ hotels worldwide, processing 70GB/min"
- Weak: "Led engineering team and managed technical architecture"

**3. The Impact on the Business** (1 clause)
What changed for the company, its users, or the market? Connect the deliverable to something a founder cares about: revenue, users, speed, cost, competitive position, team capability.

- Good: "...opening a new revenue stream for the Booking Holdings property"
- Good: "...creating 1,000+ jobs, funding schools and healthcare programs"
- Weak: "...with full GDPR/CCPA compliance" (a feature, not an impact)

### Bullet Allocation by Role Recency

- **Current/most recent roles**: fuller treatment, 3-5 sentences — this is where you prove the most
- **Mid-career roles**: 2-3 sentences, headline outcomes only
- **Early career**: 1-2 sentences, or consolidate — don't give a 2012 role the same real estate as a current one

### What to Leave Out of the Visible Summary

- Job title (already shown in the header as an inline span)
- Technology stack (already shown in skill tags below)
- Feature lists or spec sheets ("bilingual, 5 verticals, GDPR/CCPA")
- Anything that reads like a job description rather than a story
- Jargon that only makes sense to people already in the domain
- "Helped," "assisted," "contributed to" — use ownership language ("built," "led," "shipped," "drove")

### Voice and Variety

- Vary sentence openers — don't start every summary with a past-tense verb
- It's OK to start with the company or the situation instead of "Built..."
- One dash or em-dash per summary max to avoid rhythm fatigue
- Numbers land harder when surrounded by narrative, not stacked
- Keep Tom's voice human and direct — no corporate polish, no buzzword inflation
- Let the principles show through the choices highlighted, not through stated values

---

## Section Headers

Company name is the `<h3>` link. Title follows as a `<span>` — mentioned in passing, not headlined. Date range floats right.

### Context Signal

Recruiters need to classify the company in under 5 seconds. The hidden paragraph carries the full detail, but the visible summary should make the company's scale and stage obvious within the first sentence. Weave it in naturally:

- "...for the Booking Holdings property" (public company, massive scale)
- "...a 10-person startup" (early stage)
- "...100K+ MAU app" (product scale)

---

## Skill Tags

3-4 tags per role. Technologies and domains, not soft skills. Complement the summary — don't duplicate what's in the prose.

---

## Highlights & Education

- Education: degree, school, year. Brief. Certifications if relevant.
- Highlights: accelerators, competitions, press, recognition. These signal network, judgment, and market awareness.
- Advisory roles and board seats signal executive range.

---

## What This Resume Is Not

This is not a corporate CTO resume climbing toward a board seat. Tom builds things — from the Sahara to Slack-tier infrastructure — and the resume should read like someone you'd want building yours. The structure borrows from executive resume best practices (context lines, outcome-first bullets, evidence of scale) but the voice stays human, direct, and grounded in what actually shipped.
