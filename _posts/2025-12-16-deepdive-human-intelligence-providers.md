---
layout: post
title: "Deepdive: Human Intelligence Providers"
date: 2025-12-16
categories: research
---

## Human intelligence vendors deepdive (data labeling, RLHF/evals, expert networks, crowd marketplaces)

This note summarizes reputable “human intelligence” vendors—companies that provide **human labor + tooling** for tasks like data labeling, RLHF, LLM evaluations, content moderation, and research participant recruitment.

### Purpose of this deep-dive (why “human intelligence” matters)

This deep-dive is intended to:

- **Introduce the value of human intelligence in the AI industry** (in contrast to synthetic data):
  - **Ground-truth + preference data**: Humans create/validate labels, rankings, and judgments that are hard to reliably synthesize without leaking model biases back into training.
  - **Adversarial coverage**: Humans can probe edge cases, ambiguity, and “unknown unknowns” that synthetic generation tends to under-sample.
  - **Evaluation integrity**: Independent human evals can act as a check against benchmark gaming and overfitting to synthetic test sets.
  - **Domain expertise**: Some tasks require credentialed expertise (medical, legal, finance, security), where synthetic data is especially risky.
- **Clarify typical customer personas** (who buys this and why):
  - **Frontier/AI labs**: RLHF, evaluations, and specialized “frontier data” for next-model training.
  - **Enterprise AI teams**: labeling + governance + security/compliance; steady throughput at predictable quality.
  - **Product orgs**: trust & safety, moderation, multilingual QA, search relevance, and UX judgments.
  - **Research orgs**: recruitment of reliable human participants (surveys/experiments).
- **Introduce different business models** (how vendors package labor + tooling):
  - **Enterprise managed services**: sales-led delivery with SOW/MSA, SLAs, and dedicated PM/QC.
  - **Marketplace / self-serve**: requesters launch tasks; quality control is largely on the buyer.
  - **Hybrid platform + workforce**: SaaS workflow + optional vendor-provided workforce and QA.
  - **Expert contracting / “talent cloud”**: hire vetted specialists/contractors rather than buy per-label work.

### Method / caveats

- **Valuation & revenue**: public numbers (when available) are summarized in a short note **below the tables**. If no reliable public number is found, it’s treated as **Not publicly disclosed**.
- **Onboarding flows**: summarized from public product docs / “get started” guides and common enterprise procurement patterns; when vendor-specific details aren’t public, I label it as **Typical**.

### Economics snapshots (pay/earnings + market sizing)

> TODO: add sourced, public numbers for (1) typical worker earnings (expert vs microtask), and (2) market size trend (advanced LLM labeling vs simple labeling).

### Comparison table (publicly verifiable fields; “Not disclosed” means no reliable public number found)

#### Leading category

| Company | Founded | HQ region | Serving regions | Strength | Clients (examples) | Client onboarding flow | Worker onboarding workflow | Worker size (public) |
|---|---:|---|---|---|---|---|---|---|
| Surge AI (Surge Labs, Inc.) | 2020 | US (San Francisco, CA) | Global | Frontier-style RLHF + evals; high-skill judgment | AI labs (public case study: Anthropic) | Partner-managed projects **or** API/projects flow (funds required before launching to their workforce) | Managed workforce; worker pipeline details not fully public | Not publicly disclosed |
| Mercor | 2021 | US (San Francisco, CA) | Global | Expert contracting + AI-assisted matching (closer to hiring) | Not consistently public | Typical: sales/intake → define role(s) → review candidates → onboard/pay in platform | Worker: apply → interview/assessment → onboarding → paid contracting work | 30,000+ contractors (reported; see sources) |
| Scale AI | 2016 | US (SF Bay Area) | Global | Enterprise-scale labeling + compliance posture | Enterprise + public sector (public case studies) | **Typical enterprise**: sales/demo → security review → pilot → scale | **Managed workforce** + vendor QA; worker pipeline details not fully public | Not publicly disclosed |
| Amazon Mechanical Turk (MTurk) | 2005 | US (Seattle, WA) | Global | Lowest friction + low unit cost crowd microtasks | Many requesters (marketplace) | Create requester → create HIT/project → design → quals → fund → sandbox → launch | Worker signup → verify/payment setup → qualification → accept HITs | Not consistently published (marketplace; active supply fluctuates) |

#### Other reputable vendors

| Company | Founded | HQ region | Serving regions | Strength | Clients (examples) | Client onboarding flow | Worker onboarding workflow |
|---|---:|---|---|---|---|---|---|
| Appen | 1996 | Australia (Sydney) | Global | Large-scale data programs + multilingual | Big Tech historically (varies by year) | Enterprise: scope → MSA/security → pilot → ramp | Worker: apply → locale/language screening → task qualification → production + QC |
| TELUS International (AI Data Solutions) | 2005 (TELUS International) | Canada (Vancouver) / global | Global | BPO + AI data services at scale | Enterprise (public) | Enterprise: scope → contract/security → ramp | Worker: crowdsourcing + managed teams; screening/qualification varies by program |
| Sama (formerly Samasource) | 2008 | US (SF Bay Area) | Global | High-quality data labeling + impact sourcing | Public case studies | Enterprise: scope → security → pilot → scale | Worker: recruit/train (impact sourcing) → qualification → production + QC |
| iMerit | 2012 | India (Kolkata) / US presence | Global | Managed annotation + domain teams | Public case studies | Enterprise: scope → pilot → scale | Worker: hiring + training → qualification → supervised delivery |
| CloudFactory | 2010 | UK/US with Nepal roots | Global | Managed distributed workforce | Public case studies | Enterprise: scope → pilot → scale | Worker: recruit → training → QA-managed work |
| Toloka | (see sources) | Europe (reported HQ varies) | Global | Marketplace + AI data ops (strong in multilingual) | Marketplace | Self-serve + managed: project setup → pool/filters → QA → launch | Worker: signup → verification → exams/quals → tasks + ratings |
| Clickworker | 2005 | Germany (Essen) | Global | Crowd microtasks, surveys, data collection | Marketplace | Self-serve: create job → target/quals → publish → review | Worker: signup → profile/verification → quals → tasks |
| Prolific | 2014 | UK (Oxford/London, reported) | Global | High-quality research participants (academia + industry) | Researchers/companies | Self-serve: create study → screen → launch → pay | Participant: signup → ID/eligibility → take studies |
| TransPerfect DataForce | (see sources) | US (NYC for TransPerfect) | Global | Multilingual data collection + annotation | Enterprise | Enterprise: scope → contract/security → delivery | Worker: recruit panelists → consent/verification → collection + QC |
| TaskUs (AI Services) | 2008 | US (New Braunfels, TX) | Global | BPO + trust & safety + AI data operations | Enterprise | Enterprise: scope → contract/security → ramp | Worker: hiring/training → production + QA |
| Labelbox | 2018 | US (San Francisco, CA) | Global | Labeling platform + managed services | Enterprise | SaaS: signup/demo → integrate data → label/eval workflows | Workforce via partners/managed services; worker pipeline varies |
| Hive (Hive AI / Hive Data) | 2013 | US (SF Bay Area) | Global | Content moderation + labeling + model APIs | Public customers (varies) | Typical: sales/demo → pilot → scale | Mix of in-house + crowd; worker details not fully public |
| LXT | 2010 | Canada/US (reported) | Global | Speech/text data collection + annotation (multilingual) | Enterprise | Enterprise: scope → contract → collection/annotation | Worker: recruit contributors → consent/verification → tasks + QA |

**Valuation & revenue notes (publicly reported where available):** Public-company “valuation” is best treated as **market cap** (varies daily) and may not be listed here. For revenue, the only specific figures currently captured in this doc are from Wikipedia infoboxes (verify before relying on them): **Surge AI** (lists **$1.2B, 2024**), **Telus Digital / TELUS International** (lists **US$2.658B, 2024**), and **TaskUs** (lists **US$227.5M, 2024**). For Appen/TELUS/TaskUs, refer to their latest annual reports/filings for definitive revenue.

### Conclusions

#### 1) Onboarding pattern

- **Enterprise-managed (Scale-like)**: discovery call → NDA/MSA → security/compliance review → pilot → production ramp → ongoing governance/QBRs.
- **Platform-first (hybrid)**: product demo → project setup → small launch → iterate task design/QC → scale.
- **Marketplace self-serve (MTurk-like)**: account + funding → task/HIT design → qualification strategy → sandbox/soft launch → scale (buyer-owned QC).
- **Expert contracting (Mercor-like)**: role definition → candidate shortlist → interview/selection → onboarding + ongoing payments.

#### 2) Pricing / business model

- **Per-task / per-annotation**: common for labeling + microtasks; predictable unit economics but QC overhead shifts to buyer unless managed.
- **Per-hour / per-contractor / retained teams**: common for expert work, RLHF, and programs needing continuity; often sold with minimum commitments.
- **Platform fees + services**: SaaS/workflow subscription plus optional managed workforce/PM/QC.
- **Pre-funded wallets / pay-as-you-go**: common in self-serve; can be a friction point for procurement-heavy enterprises.

#### 3) Worker style

- **Open crowd marketplace** (MTurk): broad coverage and speed, but higher fraud/variance risk unless you build quals + gold + redundancy.
- **Managed workforce** (Scale/Surge pattern): tighter QC, training, and consistency; less transparency into the labor pool and often less “instant self-serve.”
- **Vetted experts / contractors** (Mercor): higher-skill judgments and domain work; lower throughput for pure microtasks, higher unit costs.

#### 4) Key pain points many vendors still don’t solve well

- **Provenance & auditability**: buyers often want cryptographic-grade lineage (who/when/how), richer adjudication logs, and reproducible labeling decisions.
- **Fraud / collusion resistance at scale**: worker identity, account resale, coordinated cheating, and model-assisted gaming remain persistent risks.
- **Fast iteration loops**: turning ambiguous specs into stable rubrics + gold sets + tooling quickly is still a heavy lift.
- **Transparent quality metrics**: many programs lack standardized, comparable metrics across vendors (inter-annotator agreement, drift, adjudication rates, error taxonomies).
- **Domain expert supply constraints**: credentialed specialists are scarce; vendors may not sustain large-scale expert throughput.
- **Data governance constraints**: some customers need strict residency/onshore-only work, short retention, and fine-grained access controls.
- **Worker experience & sustainability**: training burden, compensation fairness, and mental-health protections (esp. moderation) are uneven and hard to verify.

