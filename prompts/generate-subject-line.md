# Generate Subject Line Prompt

AI prompt for generating high-open-rate cold email subject lines.

---

## Purpose

Generate subject lines that:

- Maximize open rates (target: 40%+)
- Feel personal and relevant
- Create curiosity without being clickbait
- Avoid spam triggers
- Stay under 60 characters

---

## Prompt Template

```
ROLE:
You are an expert at writing cold email subject lines that get 
opened. You understand that the subject line's only job is to 
get the email opened — nothing more.

CONTEXT:

PROSPECT:
- Name: [First Name]
- Company: [Company Name]
- Title: [Job Title]
- Industry: [Industry]

EMAIL CONTEXT:
- Main topic: [What the email is about]
- Key hook: [Primary personalization or trigger]
- CTA type: [Meeting request / Resource share / Question]

TASK:
Generate 5 subject line options across these categories:

1. PERSONALIZED: Include prospect's name or company
2. CURIOSITY: Create an information gap
3. QUESTION: Pose a relevant question
4. DIRECT: Clear and straightforward
5. TRIGGER-BASED: Reference the specific trigger event

CONSTRAINTS:
- Maximum 60 characters (aim for 30-40)
- No spam triggers (FREE, URGENT, !!!, ALL CAPS)
- No clickbait that doesn't match email content
- Lowercase often outperforms Title Case
- Must feel human-written

OUTPUT FORMAT:
Return 5 options with character count and category label.
```

---

## Example Input

```
PROSPECT:
- Name: Sarah
- Company: TechCorp
- Title: VP of Sales
- Industry: B2B SaaS

EMAIL CONTEXT:
- Main topic: Scaling outbound personalization
- Key hook: They're hiring SDRs post-Series B
- CTA type: Meeting request
```

---

## Example Output

```
1. [PERSONALIZED] "Sarah, quick question about TechCorp's outbound" (49 chars)

2. [CURIOSITY] "noticed something about your SDR team" (38 chars)

3. [QUESTION] "scaling outbound without losing quality?" (41 chars)

4. [DIRECT] "idea for TechCorp's outbound" (28 chars)

5. [TRIGGER-BASED] "re: your Series B SDR hiring" (29 chars)
```

---

## Subject Line Formulas

### Formula 1: Name + Topic

```
{{firstName}}, [topic]
{{firstName}} — [short question]
```

**Examples:**

- "Sarah, quick question"
- "Sarah — outbound scaling"

### Formula 2: Company + Benefit

```
[benefit] for {{company}}
idea for {{company}}'s [area]
```

**Examples:**

- "idea for TechCorp's outbound"
- "thought for TechCorp"

### Formula 3: Question Format

```
[question about their challenge]?
thoughts on [topic]?
```

**Examples:**

- "scaling outbound quality?"
- "thoughts on SDR ramp time?"

### Formula 4: Trigger Reference

```
re: [trigger event]
saw [trigger] — quick thought
```

**Examples:**

- "re: your Series B"
- "saw the SDR hiring — idea"

### Formula 5: Pattern Interrupt

```
[unexpected opening]
this might be off base
random question
```

**Examples:**

- "this might be irrelevant"
- "random question for you"

---

## A/B Testing Prompts

### Test Personalization vs. Curiosity

```
Generate 2 subject line variants to A/B test:

VARIANT A: Include {{firstName}} or {{company}}
VARIANT B: Create curiosity without personalization

Same email content, different psychological approach.
```

### Test Length

```
Generate 2 subject line variants:

VARIANT A: Ultra-short (under 25 characters)
VARIANT B: Medium length (40-50 characters)

Test which length performs better for this audience.
```

### Test Question vs. Statement

```
Generate 2 subject line variants:

VARIANT A: Phrased as a question
VARIANT B: Phrased as a statement

Same core message, different framing.
```

---

## Spam Trigger Avoidance

### Words/Phrases to Avoid

```
When generating subject lines, NEVER use:
- "Free" or "Guarantee"
- "Act now" or "Limited time"
- "Click here" or "Open immediately"
- Dollar amounts or percentages
- ALL CAPS or excessive punctuation (!!!)
- "RE:" or "FWD:" when it's not a real reply
- "Urgent" or "Important"
```

### Characters to Avoid

```
Avoid:
- Multiple exclamation points
- All caps words
- Emoji (unless brand-appropriate)
- Special characters like $, %, #
```

---

## Subject Lines by Email Type

### Initial Outreach

```
Focus on: Relevance and curiosity
Examples:
- "Quick question about {{company}}"
- "{{firstName}} — thought for you"
- "idea for {{company}}'s [area]"
```

### Follow-Up #1

```
Focus on: Same thread, brief
Examples:
- "Re: [original subject]"
- "quick follow up"
- "floating this back up"
```

### Follow-Up #2 (New Angle)

```
Focus on: Fresh hook, new subject
Examples:
- "different thought for {{company}}"
- "one more idea"
- "[new angle topic]"
```

### Breakup Email

```
Focus on: Closing the loop
Examples:
- "closing the loop"
- "should I close your file?"
- "last note from me"
```

---

## Quality Checklist

Before using generated subject lines:

- [ ] Under 60 characters?
- [ ] No spam trigger words?
- [ ] Matches email content accurately?
- [ ] Would feel natural in your inbox?
- [ ] Doesn't over-promise?
- [ ] Creates appropriate curiosity?
- [ ] Variables will render correctly?

---

## Smartlead Spintax

Generate subject line variants for Smartlead:

```
Generate a single subject line with spintax variations:

Format: {option1|option2|option3}

Create variations for:
- Opening word (Quick/Brief/Short)
- Core message variations
- With/without name

Example output:
{Quick question|Brief thought|Idea} for {{company}}
```

---

## Batch Generation

For generating subject lines for multiple emails:

```
Generate subject lines for a [X]-email sequence:

EMAIL 1 (Initial): [Brief description]
EMAIL 2 (Follow-up): [Brief description]
EMAIL 3 (New angle): [Brief description]
EMAIL 4 (Breakup): [Brief description]

For each email, provide 2 subject line options.
Consider that Email 2 should use "Re:" for same thread.
```

---

## Performance Benchmarks

Use these to evaluate generated subject lines:

| Subject Line Type | Expected Open Rate |
|-------------------|-------------------|
| Personalized (name) | 40-50% |
| Question format | 35-45% |
| Curiosity gap | 35-45% |
| Direct/clear | 30-40% |
| Generic | 20-30% |

---

*Last updated: [Date]*
