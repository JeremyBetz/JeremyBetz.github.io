---
layout: page
title: Projects
permalink: /projects/
---

## Current Work

### [Moving the Defense](https://github.com/JeremyBetz/moving-the-defense)

**Status: Active research with replicated results**

An independent football tracking-data research project that measures movement by defenders nearest an off-ball attacker relative to the wider defensive unit. Across separate IDSSE and SkillCorner cohorts, straight outward movement was associated with more subsequent localized defensive reorganization than comparable movement toward goal. The directional difference replicated across seven IDSSE matches, nine original SkillCorner matches, and ten prospectively held-out SkillCorner matches. A public <a href="https://jeremybetz.github.io/moving-the-defense/">analyst demo</a> shows representative passages, diagnostic context, and rejected quality-control examples.

These are observational geometric measurements—not claims of causation, tactical value, player quality, marking responsibility, or defensive effectiveness. The work is designed to support careful follow-up analysis and video review.

### [Disrupting the Network — Analytics Cup 2.0](https://github.com/JeremyBetz/defensive-network-disruption)

**Status: Active research and experimental software**

Research for the PySport Analytics Cup 2.0 (USA Football / Defensive Positioning challenge) using permitted SkillCorner Australia A-League 2024/25 data. The project models a transparent local carrier-to-receiver option network, then evaluates whether defensive geometry improves receiver ranking beyond attacking geometry alone. On ten protected matches, adding nearest-defender geometry improved mean reciprocal rank, Hit@1, and Hit@3 in every match; a distributed-proximity refinement produced a smaller, metric-dependent gain.

The repository also includes the experimental, provider-independent <a href="https://github.com/JeremyBetz/defensive-network-disruption/releases/tag/v0.1.0">v0.1.0 Python package</a>, with synthetic examples, tests, visualization, and explicit data contracts. The results describe conditional receiver-choice ranking, not calibrated accessibility, suppression, causal defensive effects, pass success, tactical intent, player quality, or defensive value.

### Chicago Transit Data Observatory

**Status: Early-stage development**

An API-to-database analytical project organized around the question: how reliably can people move around Chicago? The intended path is API data to a database, SQL and analytical tables, then a dashboard or automated refresh. It remains early-stage rather than a finished public product.

## Selected Past Work

### [MLS International Roster Spot Valuation Tool](https://devpost.com/software/mls-international-roster-spot-valuation-tool)

**Status: Completed**

A U.S. Soccer Hackathon finalist project built with Opta data and later presented by the team at the OptaPro Forum in Chicago. I led the machine-learning work and soccer-domain framing, developed player-role clusters, and compared international-slot and domestic players within comparable tactical profiles.
