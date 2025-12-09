# Compliance Guide

Legal requirements for cold email outreach (CAN-SPAM, GDPR).

---

## Overview

Cold email is legal when done correctly. The key regulations are:

| Regulation | Region | Applies To |
|------------|--------|------------|
| CAN-SPAM | United States | All commercial email |
| GDPR | European Union | Data processing of EU residents |
| CASL | Canada | Commercial electronic messages |

**Note**: This guide covers essentials. Consult legal counsel for specific situations.

---

## CAN-SPAM Act (United States)

### Requirements

| Requirement | What It Means |
|-------------|---------------|
| **Accurate sender info** | "From" name and email must identify you/your business |
| **Honest subject lines** | Subject must reflect email content |
| **Identify as ad** | Disclose that it's a commercial message |
| **Physical address** | Include valid postal address |
| **Opt-out mechanism** | Provide clear way to unsubscribe |
| **Honor opt-outs** | Process within 10 business days |

### Penalties

- Up to **$50,120 per email** for violations
- Each email in violation = separate offense

### CAN-SPAM Compliant Email Footer

```
{{sender-name}}
{{sender-company}}
{{physical-address}}

Don't want to receive these emails? Click here to unsubscribe.
```

### What CAN-SPAM Does NOT Require

- Prior consent (opt-in) before emailing
- Disclosure of how you got their email

**Key point**: In the US, you CAN cold email without prior consent, as long as you follow the rules above.

---

## GDPR (European Union)

### When GDPR Applies

- Emailing anyone in the EU
- Processing personal data of EU residents
- Offering goods/services to EU market

### Lawful Basis for Cold Email

For B2B cold email, **"legitimate interest"** can be valid if:

1. Content is relevant to recipient's role/industry
2. You have a genuine business reason to contact them
3. You include an easy opt-out mechanism
4. You can demonstrate the relevance

### GDPR Requirements

| Requirement | Implementation |
|-------------|----------------|
| **Lawful basis** | Document your legitimate interest |
| **Transparency** | Explain how you got their data |
| **Opt-out** | Easy, free unsubscribe option |
| **Data minimization** | Only collect necessary data |
| **Right to erasure** | Delete data upon request |

### Penalties

- Up to **€20 million** or **4% of global annual revenue**
- Whichever is higher

### GDPR-Compliant Email Elements

**Opening transparency (optional but recommended):**

```
I found your contact through [LinkedIn/company website/industry directory].
```

**Footer:**

```
You're receiving this because [reason - e.g., your role as VP Sales 
at a SaaS company]. 

Unsubscribe | View our privacy policy

{{sender-company}}
{{physical-address}}
```

---

## 2025 Compliance Updates

### AI-Generated Content Disclosure

Some EU countries (Germany, France) now require:

```
This email was AI-generated. Reviewed by [Person Name].
```

**Recommendation**: If using AI to generate email content, include a human review step and consider adding disclosure for EU prospects.

### Double Opt-In Trends

GDPR enforcement is trending toward requiring double opt-in even for B2B. Best practice:

- For high-volume EU campaigns, consider an opt-in step
- For targeted, relevant B2B outreach, legitimate interest still applies

### AI-Enriched Data Scrutiny

Regulators are examining:

- How AI tools enrich contact data
- Whether data sources are legitimate
- If consent was obtained for data processing

**Best practice**: Use reputable data sources and document your data provenance.

---

## Smartlead Compliance Features

### Unsubscribe Management

Smartlead automatically:

- Adds unsubscribe links to emails
- Processes opt-out requests
- Prevents emailing unsubscribed contacts

### Configuration

1. **Settings → Unsubscribe Settings**
2. Enable automatic unsubscribe link
3. Set up unsubscribe page URL (optional custom page)

### Bounce Handling

- Hard bounces automatically removed
- Soft bounces retried then removed
- Protects sender reputation and compliance

---

## Compliance Checklist

### Every Email Must Have

- [ ] Accurate "From" name and email
- [ ] Honest subject line
- [ ] Physical postal address
- [ ] Working unsubscribe link
- [ ] Commercial message identification (if required)

### For EU Recipients (GDPR)

- [ ] Documented legitimate interest
- [ ] Explanation of data source (recommended)
- [ ] Easy opt-out mechanism
- [ ] Privacy policy link
- [ ] Process for data deletion requests

### Operational Requirements

- [ ] Honor opt-outs within 10 days (US) / promptly (EU)
- [ ] Maintain suppression list
- [ ] Document data sources
- [ ] Regular list hygiene

---

## Risk Mitigation

### Low-Risk Practices

- Target business emails (not personal)
- Ensure relevance to recipient's role
- Keep emails short and valuable
- Make unsubscribe easy and obvious
- Honor all opt-out requests immediately

### Higher-Risk (Avoid)

- Purchasing low-quality email lists
- Emailing personal email addresses
- Ignoring unsubscribe requests
- Misleading subject lines
- No physical address

---

## Templates

### US-Compliant Footer

```
{{sender-firstname}} {{sender-lastname}}
{{sender-title}}, {{sender-company}}
{{physical-address}}

Unsubscribe from future emails
```

### EU-Compliant Footer

```
{{sender-firstname}} {{sender-lastname}}
{{sender-company}}
{{physical-address}}

You received this email because of your role as {{jobTitle}} 
in the {{industry}} industry.

Unsubscribe | Privacy Policy

If you'd like your data removed from our systems, reply with 
"DELETE" and we'll process your request within 30 days.
```

---

## Quick Reference

| Question | US (CAN-SPAM) | EU (GDPR) |
|----------|---------------|-----------|
| Need prior consent? | No | No (with legitimate interest) |
| Physical address required? | Yes | Yes |
| Unsubscribe required? | Yes | Yes |
| Opt-out timeframe | 10 business days | Without undue delay |
| Can buy email lists? | Yes (with caution) | Risky |
| Personal emails OK? | Yes (follows same rules) | Higher scrutiny |

---

## Resources

- [FTC CAN-SPAM Guide](https://www.ftc.gov/business-guidance/resources/can-spam-act-compliance-guide-business)
- [GDPR Official Text](https://gdpr.eu/)
- [ICO Direct Marketing Guidance](https://ico.org.uk/for-organisations/direct-marketing/)
