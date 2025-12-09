# Campaign Configuration

Editable settings for cold email campaigns in Smartlead. Adjust these parameters for each campaign.

---

## Instructions

1. Copy this template for each new campaign
2. Fill in campaign-specific settings
3. Use as reference when setting up Smartlead campaign
4. Track what works and iterate

---

## Campaign Overview

### Campaign Details

```
Campaign Name: [Descriptive name, e.g., "Q1 2025 - VP Sales - SaaS"]
Campaign ID: [Smartlead campaign ID]
Created: [Date]
Owner: [Team member responsible]
Status: [Draft / Active / Paused / Completed]
```

### Target Audience

```
ICP Segment: [Which ICP segment from ideal-customer-profile.md]
Persona: [Primary persona, e.g., "VP of Sales"]
Industry: [Target industries]
Company Size: [Employee range]
Geography: [Regions]
```

### Goals

```
List Size: [Number of prospects]
Target Open Rate: [e.g., 50%+]
Target Reply Rate: [e.g., 5-10%]
Target Meetings: [Number of meetings to book]
```

---

## Sequence Configuration

### Sequence Structure

| Email | Purpose | Day | Time Window |
|-------|---------|-----|-------------|
| Email 1 | Initial outreach | Day 0 | [e.g., 9-11 AM] |
| Email 2 | Soft follow-up | Day [3] | [e.g., 9-11 AM] |
| Email 3 | New angle | Day [7] | [e.g., 1-3 PM] |
| Email 4 | Breakup | Day [14] | [e.g., 9-11 AM] |

### Timing Settings

```
Send Days: [e.g., Monday, Tuesday, Wednesday, Thursday]
Send Window Start: [e.g., 9:00 AM]
Send Window End: [e.g., 11:00 AM]
Timezone: [e.g., Recipient timezone / EST / PST]
```

### Delay Settings

```
Email 1 → Email 2: [3] days
Email 2 → Email 3: [4] days
Email 3 → Email 4: [7] days
```

---

## Email Configuration

### Subject Lines

```
Email 1 Subject: [Subject line with spintax]
Email 2 Subject: Re: [Same thread or new]
Email 3 Subject: [New subject line]
Email 4 Subject: [Breakup subject]
```

### From Settings

```
Sender Name: [e.g., "Alex from Acme"]
Sender Email: [e.g., alex@acme.com]
Reply-To: [If different from sender]
```

### Tracking

```
Track Opens: [Yes / No]
Track Clicks: [Yes / No - usually No for cold email]
Custom Tracking Domain: [If applicable]
```

---

## A/B Testing

### Test Variables

| Element | Variant A | Variant B | Winner |
|---------|-----------|-----------|--------|
| Subject Line | [Subject A] | [Subject B] | [TBD] |
| Opening Line | [Opening A] | [Opening B] | [TBD] |
| CTA | [CTA A] | [CTA B] | [TBD] |
| Send Time | [Time A] | [Time B] | [TBD] |

### Test Settings

```
Split: [e.g., 50/50]
Sample Size: [Minimum 100 per variant]
Success Metric: [Open rate / Reply rate / Meeting rate]
Test Duration: [e.g., 1 week minimum]
```

---

## Sending Limits

### Daily Limits (Per Email Account)

```
New emails per day: [e.g., 30-50]
Follow-ups per day: [e.g., 50-100]
Total emails per day: [e.g., 80-150]
```

### Account Warmup Status

| Email Account | Warmup Status | Daily Limit |
|---------------|---------------|-------------|
| [account1@domain.com] | [Warmed / Warming] | [X/day] |
| [account2@domain.com] | [Warmed / Warming] | [X/day] |

### Warmup Settings (If Applicable)

```
Warmup enabled: [Yes / No]
Daily warmup emails: [e.g., 20]
Warmup duration: [e.g., 2-4 weeks]
```

---

## Lead Management

### Lead Sources

```
Source 1: [e.g., Apollo export]
Source 2: [e.g., LinkedIn Sales Nav]
Source 3: [e.g., Event attendee list]
```

### Lead Qualification

```
Required fields: [firstName, lastName, email, company, customField1]
Verification: [Email verification service used]
Deduplication: [How duplicates are handled]
```

### Exclusions

```
Excluded domains: [e.g., competitor.com, gmail.com, yahoo.com]
Excluded titles: [e.g., Intern, Student]
Suppression list: [Previous contacts, existing customers]
```

---

## Reply Handling

### Auto-Stop Conditions

```
Stop on reply: [Yes]
Stop on bounce: [Yes]
Stop on unsubscribe: [Yes]
Stop on out-of-office: [Pause / Continue]
```

### Reply Categories

| Reply Type | Action | Owner |
|------------|--------|-------|
| Interested | Move to CRM, assign to AE | [Name] |
| Not interested | Mark closed, add to suppression | [Name] |
| Wrong person | Research correct contact | [Name] |
| Out of office | Pause, resume on return | [Auto] |
| Unsubscribe | Remove immediately | [Auto] |

---

## Compliance Settings

### Required Elements

```
Physical address: [Your address]
Unsubscribe link: [Enabled / Custom URL]
Company identification: [Yes]
```

### GDPR (If Targeting EU)

```
Data source disclosure: [Yes / No]
Privacy policy link: [URL]
Deletion request process: [Documented]
```

---

## Performance Tracking

### Key Metrics to Monitor

| Metric | Target | Alert Threshold |
|--------|--------|-----------------|
| Open Rate | [50%+] | [<30% = investigate] |
| Reply Rate | [5-10%] | [<2% = adjust messaging] |
| Bounce Rate | [<2%] | [>3% = pause, clean list] |
| Unsubscribe Rate | [<1%] | [>2% = review content] |
| Spam Complaint | [0%] | [Any = investigate immediately] |

### Review Schedule

```
Daily: Check bounces, spam complaints
Weekly: Review reply rates, A/B test results
Bi-weekly: Full performance review, iterate
```

---

## Campaign Checklist

### Pre-Launch

- [ ] Lead list verified and cleaned
- [ ] Custom fields populated
- [ ] Email copy reviewed and approved
- [ ] Spintax tested
- [ ] Tracking settings configured
- [ ] Sending limits set appropriately
- [ ] Suppression list updated
- [ ] Test email sent and reviewed
- [ ] Compliance elements in place

### Post-Launch (Day 1)

- [ ] Emails sending as expected
- [ ] No unusual bounce rates
- [ ] Tracking working correctly
- [ ] Reply notifications set up

### Ongoing

- [ ] Daily bounce/spam check
- [ ] Weekly performance review
- [ ] A/B tests evaluated
- [ ] Messaging iterated based on data

---

## Notes

```
[Campaign-specific notes, learnings, adjustments made]

Date: [Note]
Date: [Note]
```

---

*Last updated: [Date]*
