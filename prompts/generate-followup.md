# Generate Follow-Up Prompt

AI prompt for generating follow-up email sequences.

---

## Purpose

Generate follow-up emails that:

- Add new value with each touch
- Don't just "check in" or "follow up"
- Maintain a natural cadence
- Include a strategic breakup email
- Increase reply rates throughout the sequence

---

## Prompt Template: Full Sequence

```
ROLE:
You are an expert at writing cold email follow-up sequences. 
You understand that each follow-up must add value — never just 
"checking in." You write sequences that feel persistent but 
not pushy.

CONTEXT:

INITIAL EMAIL SUMMARY:
- Subject: [Subject line of Email 1]
- Main hook: [What Email 1 focused on]
- CTA: [What you asked for]

PROSPECT:
- Name: [First Name]
- Company: [Company Name]
- Title: [Job Title]
- Key pain point: [Main challenge]

SENDER:
- Company: [Your Company]
- Value prop: [Key benefit]
- Proof points: [2-3 customer results to draw from]

TASK:
Generate a 3-email follow-up sequence (Emails 2, 3, and 4):

EMAIL 2 (Day 3): Soft bump with one new piece of value
- Same thread (use "Re:" subject)
- Under 50 words
- Reference Email 1 briefly
- Add ONE new insight, stat, or angle

EMAIL 3 (Day 7-8): New angle
- New subject line
- Different hook than Email 1
- New value proposition or use case
- Fresh proof point
- 60-80 words

EMAIL 4 (Day 14-15): Breakup email
- Permission to close the loop
- Non-pushy tone
- Leave door open
- Under 40 words

CONSTRAINTS:
- Each email must add new value
- No "just following up" or "checking in"
- Maintain consistent tone across sequence
- Progressive urgency (soft → softer → breakup)
- All emails under 100 words

OUTPUT FORMAT:
Return all 3 emails with:
- Subject line
- Body
- Word count
- Day to send
```

---

## Example Input

```
INITIAL EMAIL SUMMARY:
- Subject: "Quick question about TechCorp's outbound"
- Main hook: Referenced their SDR hiring and Series B
- CTA: Asked if worth a quick chat

PROSPECT:
- Name: Sarah
- Company: TechCorp
- Title: VP of Sales
- Key pain point: Scaling outbound without losing quality

SENDER:
- Company: Acme
- Value prop: AI-powered personalization at scale
- Proof points: 
  1. CloudCo: 3x meetings in 90 days
  2. DataInc: 50% reduction in SDR ramp time
  3. SaaSCorp: 40% higher reply rates
```

---

## Example Output

```
EMAIL 2 (Day 3)
Subject: Re: Quick question about TechCorp's outbound

Hey Sarah,

Floating this back up.

One thing I didn't mention — we just published benchmark data 
on SDR productivity post-Series B. Happy to share if useful.

Still open to a quick chat if it makes sense.

Alex

[Word count: 42]

---

EMAIL 3 (Day 7-8)
Subject: Different angle for TechCorp

Hey Sarah,

Wanted to share a different perspective.

DataInc had a similar challenge scaling their SDR team. What 
surprised them wasn't just the meeting increase — they cut 
ramp time for new reps by 50%.

Turns out personalization at scale actually makes onboarding 
faster because reps aren't starting from scratch each time.

Worth exploring if this resonates?

Alex

[Word count: 65]

---

EMAIL 4 (Day 14-15)
Subject: Closing the loop

Hey Sarah,

Haven't heard back, so I'll assume timing isn't right.

I'll close your file for now — but feel free to reach out if 
scaling outbound becomes a priority.

Wishing you and TechCorp continued success.

Alex

[Word count: 40]
```

---

## Individual Follow-Up Prompts

### Follow-Up 2: Soft Bump

```
TASK:
Write a soft follow-up to my initial cold email.

ORIGINAL EMAIL:
[Paste or summarize Email 1]

NEW VALUE TO ADD:
[One new piece of value: stat, insight, resource, different angle]

CONSTRAINTS:
- Under 50 words
- Reference original email briefly
- Same thread (subject: "Re: [original]")
- Add the new value naturally
- Soft CTA

Don't use phrases like "just following up" or "checking in."
```

### Follow-Up 3: New Angle

```
TASK:
Write a follow-up email with a completely different angle from 
my previous emails.

PREVIOUS EMAILS SUMMARY:
- Email 1: [Main hook and CTA]
- Email 2: [What value was added]

NEW ANGLE TO EXPLORE:
[Different use case, benefit, or proof point]

CONSTRAINTS:
- New subject line (not same thread)
- 60-80 words
- Fresh hook unrelated to previous emails
- Different proof point
- Could stand alone as its own email
```

### Follow-Up 4: Breakup

```
TASK:
Write a breakup email that creates urgency without being pushy.

CONTEXT:
- Sent [X] emails with no response
- Prospect: [Name] at [Company]
- Main value prop: [What you offered]

CONSTRAINTS:
- Under 40 words
- Give them an "out" (permission to close)
- Leave door open for future
- Non-desperate tone
- Often triggers responses ("wait, don't close it!")
```

---

## Follow-Up Value-Add Ideas

### For Follow-Up 2 (Soft Bump)

```
Add ONE of these:
- Relevant stat or benchmark
- Link to useful resource
- Quick insight related to their situation
- Mention of news in their industry
- Different customer example (brief)
```

### For Follow-Up 3 (New Angle)

```
Try a completely different approach:
- Different use case for your product
- Different persona benefit (if they might forward)
- Competitive angle (without bashing)
- ROI / cost-saving angle
- Time-saving angle
- Risk-reduction angle
```

---

## Sequence Variations

### Short Sequence (3 emails total)

```
Generate a 3-email sequence (shorter than standard):

EMAIL 1: Initial outreach [provided]
EMAIL 2 (Day 4): Follow-up with new value
EMAIL 3 (Day 10): Breakup

Skip the "new angle" email for faster sequences.
```

### Extended Sequence (5 emails)

```
Generate a 5-email sequence:

EMAIL 1: Initial outreach [provided]
EMAIL 2 (Day 3): Soft bump
EMAIL 3 (Day 7): New angle #1
EMAIL 4 (Day 12): New angle #2 / social proof heavy
EMAIL 5 (Day 21): Breakup

For high-value prospects where persistence is warranted.
```

### Aggressive Sequence (Shorter Delays)

```
Generate sequence with tighter timing:

EMAIL 1: Day 0
EMAIL 2: Day 2
EMAIL 3: Day 5
EMAIL 4: Day 8

For time-sensitive offers or event-based outreach.
```

---

## Quality Checklist

For each follow-up email:

- [ ] Adds genuine new value (not just "bumping")?
- [ ] Different angle from previous emails?
- [ ] Appropriate length for its purpose?
- [ ] Tone consistent with sequence?
- [ ] CTA appropriate for this stage?
- [ ] Would not annoy recipient?

For the full sequence:

- [ ] Progressive narrative (each builds logically)?
- [ ] Variety in approach (not repetitive)?
- [ ] Breakup feels like a natural end?
- [ ] Timing appropriate for this audience?

---

## Smartlead Setup

### Sequence Timing

```
Email 1 → Email 2: 3 days
Email 2 → Email 3: 4-5 days
Email 3 → Email 4: 7 days
```

### Subject Line Threading

```
Email 1: [Unique subject]
Email 2: Re: [Email 1 subject]  ← Same thread
Email 3: [New subject]          ← New thread
Email 4: [Breakup subject]      ← New thread
```

### Variable Consistency

Ensure all emails use the same variables:

```
{{firstName}}, {{company}}, {{customField1}}, etc.
```

---

## Common Mistakes to Avoid

### Generic Follow-Ups

❌ "Just wanted to follow up on my previous email."
❌ "Checking in to see if you had a chance to review."
❌ "Bumping this to the top of your inbox."

### Guilt-Tripping

❌ "I've sent you several emails..."
❌ "Not sure if you're getting my messages..."
❌ "I'm surprised I haven't heard back..."

### Desperation

❌ "I really think this could help you..."
❌ "Please let me know either way..."
❌ "Even a quick 'not interested' would help..."

---

*Last updated: [Date]*
