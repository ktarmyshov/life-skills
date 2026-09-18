---
name: de-stromwechsel
description: Research, compare, and plan German household electricity-provider switches, especially recurring annual switches. Use for Stromanbieter search, tariff comparison, bonus and Preisgarantie checks, Ökostrom evaluation, direct-provider offer research, switching-risk analysis, Bonusjäger/Ablehnung concerns, and selection or activation of strategic reserve providers in Germany.
---

# Jährlicher Stromwechsel (DE)

Help the user choose and switch German household electricity providers with a repeatable, evidence-based process rather than blindly following comparison-portal rankings.

## Core workflow

1. Reuse context the user already supplied. Ask only for missing inputs that materially change the result:
   - supply location (at least PLZ/Ort; exact address when provider pricing or availability requires it)
   - annual consumption in kWh
   - current provider/tariff and intended switch date
   - recent provider history when available
   - switching strategy: annual optimization or longer-term stability
   - hard constraints such as max contract term, fixed-price requirement, Ökostrom preference, or excluded providers

2. Before doing market research or producing a shortlist, read [references/research-prompt.md](references/research-prompt.md) and apply its protocol to the user's current context.

3. Treat CHECK24, Verivox, and similar portals as discovery inputs, not ranking authorities. If the user supplies current portal snapshots, use them as seeds instead of repeating the same portal work unnecessarily.

4. Search provider-direct offers as well as portal-discovered tariffs. Prefer official provider documents for price, Laufzeit, Kündigung, Preisgarantie, and bonus conditions. Use independent sources for operational and complaint evidence.

5. For an intentional annual switcher:
   - optimize primarily for effective first-year cost after realistically attainable bonuses;
   - do not penalize a large bonus merely because it is large;
   - verify that bonus conditions are compatible with ordinary termination after roughly 12 months;
   - always show the no-bonus/base cost as downside and second-year context.

6. Keep financial attractiveness separate from operational reliability. Check recurring evidence around Kündigung, Zählerstand, Schätzung, Schlussrechnung, Guthaben, bonus payout, correction delays, support, and failed switches.

## Strategic reserve providers

Treat reserve providers as a provider-level risk-control mechanism, not another tariff recommendation.

- If the user does not already have reserves, identify 1–2 providers worth preserving as strategic reserves.
- Choose reserves for dependable fallback, not for the lowest first-year price.
- A reserve should have broadly reasonable market pricing and be acceptable to stay with for roughly 2–3 years if optimization becomes unreliable.
- Prefer operational stability, broad availability, straightforward contracts, and a sensible non-promotional price structure.
- Consider diversification such as a local/regional Stadtwerk plus a larger provider when it improves resilience, but do not force this pattern.
- Account for provider history. A provider already used or recently burned for a promotion may be a weaker reserve.
- Once designated, exclude a reserve provider from the normal annual-switch candidate pool even if it temporarily becomes attractive.
- Activate a reserve only when repeated rejections, clear frequent-switcher friction, or other market failures make further optimization unattractive. Roughly 2–3 failed applications can be a practical trigger, but use judgment.

When a reserve is activated, switch the objective from **optimize** to **stabilize**: choose a suitable ordinary tariff from that provider and accept a reasonable price premium in exchange for reliability.

## Output

Keep the decision practical:

- state assumptions and any missing data;
- return no more than 3–5 normal candidates unless the user asks for more;
- show first-year effective cost, base/no-bonus cost, key terms, bonus safety, Ökostrom quality when relevant, operational risk, and important caveats;
- list strategic reserve providers separately and mark them as **do not use in normal switching**;
- include attractive near-misses or rejected candidates when the rejection reason teaches something important;
- give the concrete next step for contract verification or Abschluss.

At the end of a completed switching cycle, remind the user to consider preserving useful history for the next cycle: chosen provider, actual cost, bonuses, acceptance/rejection, Kündigung outcome, meter-reading or billing issues, and reserve-provider choices. Do not impose a storage format; let the user choose a spreadsheet, Markdown, notes, another system, or nothing.

Respond in the user's language. Preserve German market and legal terms where they are clearer than translations.
