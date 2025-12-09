# Generate Icebreaker Prompt

AI prompt for generating personalized opening lines for cold emails.

---

## Purpose

Generate a personalized 1-2 sentence icebreaker that:

- References specific, verifiable information about the prospect
- Feels genuinely researched, not generic
- Naturally transitions to a business context
- Avoids flattery or over-personalization

---

## Prompt Template

Copy and customize this prompt for your AI tool:

```
ROLE:
You are an expert B2B cold email copywriter. Your specialty is 
writing personalized opening lines that feel genuinely researched 
and human-written.

CONTEXT:
I'm reaching out to a prospect with the following details:

PROSPECT INFORMATION:
- Name: [First Name] [Last Name]
- Title: [Job Title]
- Company: [Company Name]
- Industry: [Industry]
- Company Size: [Employee Count]

RESEARCH FINDINGS:
- Recent LinkedIn Post/Activity: [Description of post or activity]
- Company News: [Recent news, funding, launches, etc.]
- Trigger Event: [What prompted this outreach]
- Other Notable Info: [Any other relevant details]

MY COMPANY:
- What we do: [One-liner about your company]
- How we help: [Relevant benefit for this prospect]

TASK:
Generate 3 personalized icebreaker options (1-2 sentences each) that:

1. Reference the research findings naturally
2. Show genuine interest, not generic flattery
3. Could transition smoothly into a business conversation
4. Feel human-written, not AI-generated
5. Are specific enough that they couldn't apply to anyone else

CONSTRAINTS:
- Maximum 30 words per icebreaker
- No buzzwords or corporate jargon
- No over-the-top compliments ("I'm a huge fan of your work!")
- Must reference verifiable information
- Conversational tone

OUTPUT FORMAT:
Return 3 options, numbered 1-3, with a brief note on when each works best.
```

---

## Example Input

```
PROSPECT INFORMATION:
- Name: Sarah Chen
- Title: VP of Sales
- Company: TechCorp
- Industry: B2B SaaS
- Company Size: 250 employees

RESEARCH FINDINGS:
- Recent LinkedIn Post: Posted about the challenge of scaling SDR 
  teams without losing personalization quality
- Company News: Raised Series B ($30M) 2 months ago
- Trigger Event: Hiring 5 SDRs based on LinkedIn Jobs
- Other: Previously worked at Salesforce

MY COMPANY:
- What we do: AI-powered sales engagement platform
- How we help: Helps sales teams personalize outreach at scale
```

---

## Example Output

```
1. "Saw your post on scaling SDR quality vs. quantity — that tension 
   is real, especially post-Series B when the pressure to grow is intense."
   
   Best for: When their LinkedIn post is highly relevant to your solution

2. "Congrats on the Series B and the SDR hiring push. The 'scale without 
   losing quality' challenge is one we hear constantly at this stage."
   
   Best for: When funding + hiring creates a clear trigger event

3. "Your point about personalization suffering as teams scale really 
   resonated — it's the #1 thing sales leaders mention when we talk."
   
   Best for: When you want to validate their perspective and build rapport
```

---

## Variations by Scenario

### When You Have Strong LinkedIn Activity

```
Focus the prompt on:
- Specific posts they've written
- Topics they engage with
- Opinions they've shared

Example addition to prompt:
"Prioritize referencing their LinkedIn post about [topic]. 
Make it clear you actually read and understood their point."
```

### When You Have Company News

```
Focus the prompt on:
- Funding announcements
- Product launches
- Expansion news
- Leadership changes

Example addition to prompt:
"Reference the [news event] and connect it to a challenge 
they're likely facing as a result."
```

### When You Have Mutual Connections

```
Focus the prompt on:
- Shared connections
- Same previous employer
- Same school/program
- Same community/group

Example addition to prompt:
"Lead with the mutual connection point, but keep it brief 
and transition quickly to relevance."
```

### When Research is Limited

```
Focus the prompt on:
- Role-based relevance
- Industry trends
- Common challenges for their position

Example addition to prompt:
"With limited specific research, focus on role-based relevance. 
Reference a common challenge for [their title] in [their industry]."
```

---

## Quality Checklist

Before using generated icebreakers:

- [ ] Is the referenced information verifiable and accurate?
- [ ] Would this feel natural coming from a human?
- [ ] Is it specific to THIS prospect (not generic)?
- [ ] Does it avoid over-the-top flattery?
- [ ] Does it naturally lead to a business conversation?
- [ ] Is it under 30 words?

---

## Anti-Patterns to Avoid

### Too Generic

❌ "Hope you're having a great week!"
❌ "I came across your profile and was impressed."
❌ "Your company looks like it's doing great things."

### Too Flattering

❌ "I'm a huge fan of your work and have followed you for years."
❌ "Your LinkedIn posts are always so insightful."
❌ "TechCorp is truly revolutionizing the industry."

### Too Salesy

❌ "I noticed you might benefit from our solution."
❌ "Companies like yours typically struggle with..."
❌ "I wanted to introduce you to a game-changing platform."

### Too Creepy

❌ "I saw you were in San Francisco last Tuesday."
❌ "Congrats on your daughter's graduation!"
❌ "I noticed you liked [specific personal post]."

---

## Smartlead Integration

Store generated icebreakers in `{{customField3}}`:

```
{{customField3}}

[Rest of email body]
```

### Fallback for Empty Icebreakers

```
{{{customField3}}|Noticed {{company}} has been growing fast lately — 
always interesting to see how teams scale their outreach at this stage.}
```

---

## Batch Generation Workflow

For generating icebreakers at scale:

1. **Export prospect list** with research data
2. **Create a spreadsheet** with columns:
   - Prospect info
   - Research findings
   - Generated icebreaker
3. **Run prompt for each prospect** (or batch of 5-10)
4. **Review and edit** generated content
5. **Import to Smartlead** as custom field

---

*Last updated: [Date]*
