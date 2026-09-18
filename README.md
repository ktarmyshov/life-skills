# Life Skills

Practical AI skills for real-life decisions and procedures.

This repository is for reusable operating procedures where a general AI benefits from domain-specific workflow, failure modes, and decision logic — especially tasks people perform only occasionally and should not need to become experts in.

## Skills

| Skill | Display name | Purpose |
| --- | --- | --- |
| [`de-stromwechsel`](skills/de/de-stromwechsel/) | **Jährlicher Stromwechsel (DE)** | Research and plan German household electricity switches, including direct offers, bonus safety, operational risks, and strategic reserve providers. |

## Install

List the skills available in this repository:

```bash
npx skills add ktarmyshov/life-skills --list
```

Install one skill:

```bash
npx skills add ktarmyshov/life-skills --skill de-stromwechsel
```

## Structure

Country-specific skills are grouped by country. The skill folder itself keeps the full skill name so it follows the Agent Skills naming convention.

```text
skills/
  de/
    de-stromwechsel/
      SKILL.md
      agents/
        openai.yaml
      references/
        research-prompt.md
```

General-purpose skills can live in a separate non-country-specific group as the collection grows.

## Design principle

A useful life skill should add more than a generic prompt. It should preserve non-obvious procedure, domain lessons, failure modes, or decision logic that materially improves the result after competent use of a general AI.
