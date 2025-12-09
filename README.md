# Cold Email Playbook

> A comprehensive guide for creating high-converting cold email campaigns using Smartlead. Best practices, templates, and AI prompts for personalized outreach at scale.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Smartlead](https://img.shields.io/badge/Platform-Smartlead-orange)](https://smartlead.ai)

## Overview

This playbook provides everything you need to run effective cold email campaigns:

- **Best Practices** - Research-backed strategies for subject lines, copy, personalization, sequences, and compliance
- **Context Templates** - Fill-in documents for your ICP, value proposition, and company info
- **Input Templates** - Editable fields for prospect data and campaign configuration
- **AI Prompts** - Structured prompts for generating personalized email content at scale

## Directory Structure

```
├── best-practices/     # Guidelines and proven strategies
├── context/            # Background information for email generation
├── inputs/             # Editable fields and templates
└── prompts/            # AI prompts for content generation
```

## Quick Start

1. **Set up context** - Fill in the templates in `/context/` with your company and ICP details
2. **Review best practices** - Read through `/best-practices/` to understand proven strategies
3. **Prepare inputs** - Use `/inputs/` to define prospect variables and campaign settings
4. **Generate content** - Use `/prompts/` with AI to create personalized email content

---

## Best Practices

| File | Description |
|------|-------------|
| [01-fundamentals.md](best-practices/01-fundamentals.md) | Core principles of effective cold email |
| [02-subject-lines.md](best-practices/02-subject-lines.md) | Crafting high-open-rate subject lines |
| [03-email-copy.md](best-practices/03-email-copy.md) | Writing compelling email body content |
| [04-personalization-ai.md](best-practices/04-personalization-ai.md) | AI-powered personalization with Smartlead |
| [05-sequences-timing.md](best-practices/05-sequences-timing.md) | Sequence structure and optimal timing |
| [06-compliance.md](best-practices/06-compliance.md) | Legal requirements (CAN-SPAM, GDPR) |

## Context (Fill These In)

| File | Description |
|------|-------------|
| [ideal-customer-profile.md](context/ideal-customer-profile.md) | Define your target persona and company profile |
| [value-proposition.md](context/value-proposition.md) | Your product benefits and differentiators |
| [company-info.md](context/company-info.md) | Sender company details and credibility |
| [industry-pain-points.md](context/industry-pain-points.md) | Common challenges and trigger events |
| [competitor-landscape.md](context/competitor-landscape.md) | Positioning against alternatives |

## Inputs (Editable Per Campaign)

| File | Description |
|------|-------------|
| [prospect-variables.md](inputs/prospect-variables.md) | Per-prospect data fields |
| [email-templates.md](inputs/email-templates.md) | Skeleton structures for emails |
| [personalization-data.md](inputs/personalization-data.md) | Data points to research per prospect |
| [campaign-config.md](inputs/campaign-config.md) | Campaign settings and timing |

## AI Prompts

| File | Description |
|------|-------------|
| [generate-icebreaker.md](prompts/generate-icebreaker.md) | Generate personalized opening lines |
| [generate-email-body.md](prompts/generate-email-body.md) | Generate full email content |
| [generate-subject-line.md](prompts/generate-subject-line.md) | Generate high-converting subject lines |
| [generate-followup.md](prompts/generate-followup.md) | Generate follow-up sequences |

---

## Smartlead Integration

This playbook is designed specifically for use with [Smartlead](https://smartlead.ai). Key Smartlead features referenced:

### Variables

- `{{firstName}}`, `{{lastName}}`, `{{company}}` - Standard contact fields
- `{{sl_time_of_day}}` - Dynamic greeting (morning/afternoon/evening)
- `{{sl_day_of_week}}` - Current day name
- `{{sl_date "X days from now" "format"}}` - Date suggestions
- `{{customField1}}` through `{{customField20}}` - Custom data fields

### Spintax

Use `{option1|option2|option3}` syntax to create variations:

```
{Hi|Hello|Hey} {{firstName}}, {hope you're doing well|hope your week is going great}
```

---

## Key Metrics to Target

| Metric | Target | Notes |
|--------|--------|-------|
| Open Rate | 40-60% | Subject line dependent |
| Reply Rate | 5-15% | Personalization dependent |
| Bounce Rate | <2% | List hygiene critical |
| Meeting Book Rate | 1-3% | Full funnel optimization |

---

## Usage with AI

The `/prompts/` directory contains structured prompts for AI-assisted email generation. Each prompt includes:

1. **System context** - Role and constraints for the AI
2. **Input requirements** - What data to provide
3. **Output format** - Expected structure of generated content
4. **Examples** - Sample inputs and outputs

Feed the context files and prospect data to these prompts for consistent, high-quality email generation.

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/OffDeckProductStudio/cold-email-playbook.git
cd cold-email-playbook
```

### 2. Fill in Your Context

Start by completing the templates in `/context/`:

1. `ideal-customer-profile.md` - Define who you're targeting
2. `value-proposition.md` - Document your benefits and proof points
3. `company-info.md` - Your company details for credibility

### 3. Configure Your Campaign

Use `/inputs/` to set up your campaign:

1. Map your prospect data to Smartlead variables
2. Customize email templates with your messaging
3. Configure timing and sequence settings

### 4. Generate Content with AI

Use the prompts in `/prompts/` with your AI tool of choice (Claude, GPT-4, etc.) to generate:

- Personalized icebreakers
- Full email bodies
- Subject line variations
- Follow-up sequences

---

## Contributing

Contributions are welcome! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Built by [OffDeck Product Studio](https://offdeck.com)
