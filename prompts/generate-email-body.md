# Generate Email Body Prompt

AI prompt for generating complete cold email body content.

---

## Purpose

Generate a full cold email that:

- Opens with a personalized hook
- Addresses a relevant pain point
- Presents your solution with proof
- Ends with a clear, low-friction CTA
- Stays under 125 words

---

## Prompt Template

```
ROLE:
You are an expert B2B cold email copywriter. You write concise, 
personalized emails that get responses. You never use buzzwords, 
jargon, or corporate speak.

CONTEXT:

PROSPECT:
- Name: [First Name]
- Title: [Job Title]
- Company: [Company Name]
- Industry: [Industry]
- Company Size: [Size]

RESEARCH:
- Trigger Event: [What prompted outreach]
- Pain Points: [Likely challenges based on role/situation]
- Recent Activity: [LinkedIn post, news, etc.]

SENDER:
- Company: [Your Company]
- What We Do: [One-liner]
- Key Benefit: [Primary outcome you deliver]
- Proof Point: [Customer result or social proof]
- Sender Name: [Your name]

TASK:
Write a cold email with the following structure:

1. OPENING (1-2 sentences): Personalized hook referencing research
2. PAIN (1-2 sentences): Acknowledge their likely challenge
3. SOLUTION (1-2 sentences): How you help, with proof point
4. CTA (1 sentence): Clear, low-friction ask

CONSTRAINTS:
- Total length: 50-125 words (6-8 sentences max)
- Tone: Conversational, direct, human
- No buzzwords: Avoid "leverage," "synergy," "revolutionary," etc.
- No feature dumps: Focus on outcomes
- One CTA only: Make it easy to respond
- Plain text: No formatting, bullets, or links in body

OUTPUT FORMAT:
Return the email body only (no subject line). Include a word count.
```

---

## Example Input

```
PROSPECT:
- Name: Sarah
- Title: VP of Sales
- Company: TechCorp
- Industry: B2B SaaS
- Company Size: 250 employees

RESEARCH:
- Trigger Event: Hiring 5 SDRs, just raised Series B
- Pain Points: Scaling outbound without losing personalization quality
- Recent Activity: Posted about quality vs. quantity in sales outreach

SENDER:
- Company: Acme
- What We Do: AI-powered sales engagement platform
- Key Benefit: Personalize outreach at scale without manual effort
- Proof Point: CloudCo increased meetings booked by 3x in 90 days
- Sender Name: Alex
```

---

## Example Output

```
Hey Sarah,

Saw your post on scaling SDR quality vs. quantity — that tension 
is real, especially when you're hiring fast post-Series B.

Most sales leaders I talk to at this stage hit the same wall: 
more reps, more emails, but reply rates start to tank.

We helped CloudCo solve this — they went from struggling to 
scale to booking 3x more meetings in 90 days without adding 
headcount.

Worth a quick chat to see if we could help TechCorp do the same?

Alex

[Word count: 84]
```

---

## Variations by Email Type

### Initial Outreach (Standard)

Use the main prompt template above.

### Referral-Based Email

Add to prompt:

```
REFERRAL CONTEXT:
- Referred by: [Name]
- Relationship: [How referrer knows prospect]
- What referrer said: [Brief context]

Adjust the opening to lead with the referral naturally, 
not in a forced way like "John told me to reach out."
```

### Trigger Event Email

Add to prompt:

```
TRIGGER FOCUS:
The trigger event ([specific event]) should be the primary hook. 
Connect the trigger directly to a pain point they're likely 
experiencing as a result.
```

### Value-First Email

Add to prompt:

```
VALUE-FIRST APPROACH:
Instead of asking for a meeting, offer something valuable first:
- Resource: [e.g., guide, template, benchmark data]
- Insight: [e.g., observation about their situation]

The CTA should be about sharing the value, not booking a call.
```

---

## Prompt Modifiers

### For Different Tones

**More Casual:**

```
Additional instruction: Write in a very casual, friendly tone. 
Use contractions freely. Imagine emailing a colleague you've 
met at a conference.
```

**More Formal:**

```
Additional instruction: Write in a professional but warm tone. 
Suitable for C-suite executives at enterprise companies.
```

### For Different CTAs

**Soft CTA:**

```
CTA instruction: Use a very soft CTA like "Curious if this 
resonates?" or "Worth exploring?"
```

**Direct CTA:**

```
CTA instruction: Use a direct CTA asking for a specific time, 
like "Do you have 15 minutes Thursday or Friday?"
```

### For Different Lengths

**Ultra-Short (Under 50 words):**

```
Length constraint: Keep the entire email under 50 words. 
Cut everything non-essential. Prioritize: hook, one value point, CTA.
```

**Longer (100-150 words):**

```
Length constraint: You have room for 100-150 words. Include 
more context and a second proof point, but don't add fluff.
```

---

## Quality Checklist

Before sending generated email:

- [ ] Under 125 words?
- [ ] Opening references specific research?
- [ ] Pain point is relevant to their role/situation?
- [ ] Solution focuses on outcomes, not features?
- [ ] Proof point is specific (company name, metric)?
- [ ] Single, clear CTA?
- [ ] No buzzwords or jargon?
- [ ] Reads naturally when spoken aloud?
- [ ] Would YOU reply to this email?

---

## Common Issues and Fixes

### Email Too Long

**Fix:** Add to prompt:

```
The email is too long. Cut it to under [X] words. Remove any 
sentence that doesn't directly serve: hook, pain, solution, or CTA.
```

### Too Generic

**Fix:** Add more specific research to the prompt, or:

```
This is too generic. Make the opening line specific to 
[exact detail from research]. The prospect should feel like 
this email was written just for them.
```

### Too Salesy

**Fix:** Add to prompt:

```
This sounds too salesy. Rewrite to sound like a peer reaching 
out to share something relevant, not a salesperson pitching.
```

### Weak CTA

**Fix:** Add to prompt:

```
The CTA is weak. Rewrite with a clearer ask that makes it 
easy to say yes. Options: "Worth a quick chat?" / "Open to 
learning more?" / "15 min this week?"
```

---

## Batch Generation

For generating multiple emails:

```
BATCH INSTRUCTIONS:
Generate emails for the following [X] prospects. Use the same 
sender information and overall structure, but personalize 
each email based on the prospect's specific details.

[Prospect 1 data]
[Prospect 2 data]
[Prospect 3 data]

Return each email separately with the prospect name as header.
```

---

## Smartlead Integration

### Variable Placement

```
{{sl_time_of_day}} {{firstName}},

{{customField3}}

[AI-generated body with {{company}} and other variables]

{{sender-firstname}}
```

### Spintax for Variation

Add to prompt:

```
Include spintax variations for:
- Greeting: {Hi|Hey|Hello}
- CTA: {Worth a chat?|Open to connecting?|Interested in learning more?}

Format spintax like: {option1|option2|option3}
```

---

*Last updated: [Date]*
