# Sequences and Timing

How to structure follow-up sequences and optimize send timing in Smartlead.

---

## The Science of Follow-Ups

- **60%+ of meetings** are booked after the 2nd or 3rd email
- First follow-up boosts reply rates by **up to 49%**
- Second follow-up adds approximately **3% more replies**
- Beyond 3-4 emails, diminishing returns set in

**Bottom line**: Most deals require persistence, but respect boundaries.

---

## Optimal Sequence Length

| Sequence Type | Emails | Best For |
|---------------|--------|----------|
| Short | 3 emails | Warm leads, referrals |
| Standard | 4-5 emails | Cold outreach |
| Extended | 6-7 emails | High-value targets |

### Recommended: 4-Email Sequence

| Email | Purpose | Days After Previous |
|-------|---------|---------------------|
| Email 1 | Initial outreach | Day 0 |
| Email 2 | Soft follow-up | Day 3 |
| Email 3 | New angle/value | Day 4-5 |
| Email 4 | Breakup email | Day 7-10 |

---

## Timing Between Emails

### Recommended Cadence

```
Email 1: Day 0 (Initial send)
    ↓ 3 days
Email 2: Day 3 (First follow-up)
    ↓ 4-5 days
Email 3: Day 7-8 (Second follow-up)
    ↓ 5-7 days
Email 4: Day 14-15 (Breakup)
```

### Why This Works

- **3 days**: Gives time to read, not so long they forget
- **4-5 days**: Shows persistence without desperation
- **7+ days**: Final touches feel less pushy

### Cadence Variations

**Aggressive (High-urgency offers):**

```
Day 0 → Day 2 → Day 4 → Day 7
```

**Relaxed (Enterprise/Senior executives):**

```
Day 0 → Day 5 → Day 10 → Day 21
```

---

## Best Days and Times

### Best Days to Send

| Day | Performance | Notes |
|-----|-------------|-------|
| Tuesday | Excellent | Peak engagement |
| Wednesday | Excellent | Consistent opens |
| Thursday | Good | Strong, tapers end of week |
| Monday | Moderate | Inbox overload from weekend |
| Friday | Low | Weekend mindset |
| Weekend | Poor | Avoid unless specific reason |

### Best Times to Send

| Time Window | Performance | Why |
|-------------|-------------|-----|
| 9:00-11:00 AM | Excellent | Morning inbox check |
| 1:00-3:00 PM | Good | Post-lunch productivity |
| 7:00-8:00 AM | Moderate | Early risers, less competition |
| 4:00-6:00 PM | Low | End-of-day rush |

### Timezone Considerations

- **Always send in recipient's timezone**
- Smartlead handles this automatically if timezone data is included
- Default to EST/PST for US prospects if unknown

---

## Email-by-Email Strategy

### Email 1: Initial Outreach

**Purpose**: Introduce yourself, establish relevance, make the ask

**Structure:**

```
- Personalized opening (reference trigger/research)
- Pain point acknowledgment
- Brief value proposition
- Soft CTA
```

**Example:**

```
Subject: Quick question about {{company}}'s outbound

{{sl_time_of_day}} {{firstName}},

{{customField1_icebreaker}}

Most [their role] I talk to are wrestling with [pain point] 
as they scale.

We helped [Similar Company] solve this and [specific result].

Worth a quick chat?

{{sender-firstname}}
```

---

### Email 2: Soft Follow-Up (Day 3)

**Purpose**: Gentle reminder, add slight value

**Structure:**

```
- Brief reference to Email 1
- Quick value add (insight, stat, or different angle)
- Restate CTA
```

**Example:**

```
Subject: Re: Quick question about {{company}}'s outbound

Hi {{firstName}},

Wanted to float this back up.

One thing I forgot to mention — [additional insight or stat 
relevant to their situation].

Thought it might be useful context. Still happy to chat if 
it makes sense.

{{sender-firstname}}
```

**Key points:**

- Same thread (use "Re:")
- Under 50 words
- Add ONE new piece of value

---

### Email 3: New Angle (Day 7-8)

**Purpose**: Try a different hook, provide more value

**Structure:**

```
- New opening (don't reference previous emails)
- Different value proposition or use case
- Social proof
- Clear CTA
```

**Example:**

```
Subject: Idea for {{company}}

Hi {{firstName}},

Came across this [resource/insight] that made me think of 
{{company}}'s [situation/initiative].

[Brief insight or how others in their position benefited]

[Case study: Similar Company saw X result]

Would it help to see how they did it?

{{sender-firstname}}
```

**Key points:**

- Fresh subject line
- Different angle than Email 1
- More substantial value

---

### Email 4: Breakup Email (Day 14-15)

**Purpose**: Create urgency, permission to close the loop

**Structure:**

```
- Acknowledge lack of response
- Offer to close the loop
- Leave door open
```

**Example:**

```
Subject: Should I close your file?

Hi {{firstName}},

I haven't heard back, so I'll assume the timing isn't right.

I'll close out your file for now, but feel free to reach out 
if [pain point] becomes a priority.

Wishing you and the {{company}} team continued success.

{{sender-firstname}}
```

**Key points:**

- Non-pushy tone
- Gives them an "out"
- Often triggers responses ("wait, don't close it!")

---

## Smartlead Sequence Setup

### Creating a Sequence

1. **Campaign → New Campaign**
2. **Add Email Steps** with delays between each
3. **Set send windows** (e.g., 9 AM - 11 AM)
4. **Enable timezone detection** for recipient-based timing

### Delay Settings

| Between | Recommended Delay |
|---------|-------------------|
| Email 1 → 2 | 3 days |
| Email 2 → 3 | 4-5 days |
| Email 3 → 4 | 7 days |

### Send Window Configuration

```
Days: Monday, Tuesday, Wednesday, Thursday
Time: 9:00 AM - 11:00 AM (recipient timezone)
Daily limit: Based on email account warmup status
```

---

## Sequence Variations by Persona

### C-Suite Executives

- Longer delays (5-7 days between)
- Shorter emails
- Focus on strategic outcomes
- 3 emails max

### Mid-Level Managers

- Standard cadence (3-5 days)
- More tactical value
- 4-5 emails acceptable

### Individual Contributors

- Can be slightly more frequent
- Technical details welcome
- 4-5 emails standard

---

## A/B Testing Sequences

### What to Test

| Element | Variation A | Variation B |
|---------|-------------|-------------|
| Sequence length | 3 emails | 5 emails |
| Timing | 3-day gaps | 5-day gaps |
| Breakup email | Include | Exclude |
| Email 2 approach | Soft reminder | New value |

### Measurement

Track per sequence variant:

- Reply rate
- Positive reply rate
- Meeting book rate
- Unsubscribe rate

---

## When to Stop Emailing

### Stop Signals

- Explicit opt-out request
- Bounce (hard bounce = remove immediately)
- "Not interested" reply
- Out-of-office indicating role change

### Pause Signals

- Out-of-office (resume after their return)
- "Not right now" (add to nurture list)
- No response after full sequence (wait 90 days before re-engaging)

---

## Sequence Checklist

Before launching:

- [ ] 3-5 emails in sequence?
- [ ] 3-7 day delays between emails?
- [ ] Each email adds new value?
- [ ] Breakup email included?
- [ ] Send window set to business hours?
- [ ] Timezone detection enabled?
- [ ] Daily limits appropriate for account warmup?
- [ ] Unsubscribe link included?
