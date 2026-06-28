# Arabic Content Creator Skill

A reusable LLM skill for generating high-quality Arabic business content tailored to Saudi Arabian and Middle Eastern technology markets.

## Install via Claude Code

```bash
# From GitHub (recommended)
npx skills add EngOREOO/content-creator-skill -g -y

# Or from npm
npx skills add @engoreeo/arabic-content-creator-skill -g -y
```

Then activate with `/arabic` in any Claude Code conversation.

## Files

| File | Description |
|------|-------------|
| `SKILL.md` | opencode-compatible skill file (entry point for `npx skills add`) |
| `arabic-content-skill.md` | Main skill file (907 lines) — drop into any LLM |
| `scoring-engine.md` | 0–100 evaluation system (689 lines) |
| `research/` | Full research datasets (analysis, patterns, localization guide, style guide, blacklist) |

## Marketplace

This skill is available on the [Claude Marketplace](https://github.com/EngOREOO/content-creator-skill) — install it in Claude Code with `npx skills add EngOREOO/content-creator-skill -g -y`.

## What It Does

This skill transforms any LLM into an **Arabic content strategist and copywriter** specialized in:
- Software houses, AI companies, SaaS, cybersecurity, and digital agencies
- Saudi Arabian, UAE, and broader Middle Eastern markets
- Bilingual Arabic-English content optimized for conversion and SEO
- Vision 2030-aligned messaging and Saudi localization

## 10-Phase Research Behind the Skill

The skill was built from a systematic analysis of **234 Middle Eastern tech companies** across 7 countries (SA, UAE, QA, KW, BH, EG, JO) and 11 industry categories. The research included website crawling, writing analysis, linguistic dataset creation (225+ headline patterns, 150+ CTAs, 51+ hero structures), Saudi localization study, and negative pattern detection.

---

## How to Use With Different LLMs

### Claude Code (recommended)

**Option A — Skill file (recommended):**
1. Copy `arabic-content-skill.md` to `~/.claude/skills/arabic-content-creator/SKILL.md`
2. Claude auto-loads it when the task matches content creation
3. Or use `/skill arabic-content-creator` to activate it

**Option B — System prompt:**
Paste the entire `arabic-content-skill.md` content into a Project's Custom Instructions or as a system prompt.

### ChatGPT

1. Open **Settings → Personalization → Custom Instructions**
2. Paste the `arabic-content-skill.md` content into the "What would you like ChatGPT to know?" section
3. Or create a **GPT** (Builder) and paste the skill into the Instructions field

### Gemini

1. Use **Gems** feature (if available)
2. Create a new Gem and paste the skill content as instructions
3. Or include it in the system instruction field via API

### Any LLM API (OpenAI, Anthropic, Google, Together, etc.)

```python
system_prompt = open("arabic-content-skill.md").read()
response = client.chat.completions.create(
    model="gpt-4o",
    messages=[
        {"role": "system", "content": system_prompt},
        {"role": "user", "content": "Write a homepage hero section for a Saudi AI company..."}
    ]
)
```

### 5-Minute Quick Start

1. Load the skill into your LLM (see above)
2. Give it a brief like: *"Write an About Us page in Arabic for a Riyadh-based cybersecurity company targeting government clients. Include Vision 2030 alignment."*
3. The skill will:
   - Think through audience, tone, structure
   - Write the content with proper Saudi localization
   - Self-review against 55 quality checkpoints
   - Score it 0–100
   - Rewrite if below 95

### Scoring Your Content

Use `scoring-engine.md` to evaluate any Arabic content:

```
Using the scoring engine, evaluate this text:
[Paste text here]
```

The engine scores across 9 dimensions: Naturalness, Saudi Localization, Persuasiveness, SEO, Authority, Clarity, Readability, Conversion, Originality.

---

## Usage Examples

**"Write a hero section for a Jeddah-based web development company"**

**"Create 5 Arabic LinkedIn posts about digital transformation in Saudi Arabia"**

**"Translate and localize this SaaS landing page for the Saudi market"**

**"Generate a case study for a Saudi AI company that helped a bank reduce fraud"**

**"Evaluate this Arabic homepage and score it using the scoring engine"**

---

## License

MIT
