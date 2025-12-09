# Prospect Variables

Define the data fields collected for each prospect. These map to Smartlead variables for email personalization.

---

## Instructions

1. Define which fields you collect for each prospect
2. Map fields to Smartlead variables
3. Specify which fields are required vs. optional
4. Document data sources for enrichment

---

## Smartlead Variable Mapping

### Standard Fields

| Field Name | Smartlead Variable | Required | Data Type |
|------------|-------------------|----------|-----------|
| First Name | `{{firstName}}` | Yes | Text |
| Last Name | `{{lastName}}` | Yes | Text |
| Email | Email field | Yes | Email |
| Company | `{{company}}` | Yes | Text |

### Custom Fields (Up to 20)

| Field Name | Smartlead Variable | Required | Purpose |
|------------|-------------------|----------|---------|
| Job Title | `{{customField1}}` | Yes | Role-based messaging |
| LinkedIn URL | `{{customField2}}` | Recommended | Research reference |
| Icebreaker | `{{customField3}}` | Recommended | AI-generated personalization |
| Company Size | `{{customField4}}` | Optional | Segmentation |
| Industry | `{{customField5}}` | Optional | Industry-specific messaging |
| Pain Point | `{{customField6}}` | Optional | AI-generated |
| Trigger Event | `{{customField7}}` | Optional | Timely reference |
| Tech Stack | `{{customField8}}` | Optional | Relevance signal |
| Recent News | `{{customField9}}` | Optional | Personalization hook |
| Case Study Match | `{{customField10}}` | Optional | Social proof |

---

## Field Definitions

### Required Fields

#### First Name

```
Variable: {{firstName}}
Format: Text, capitalized
Example: "Sarah"
Fallback: "there" (if missing)
Source: Lead list, LinkedIn
```

#### Last Name

```
Variable: {{lastName}}
Format: Text, capitalized
Example: "Chen"
Fallback: None (don't use if missing)
Source: Lead list, LinkedIn
```

#### Email

```
Variable: [Smartlead email field]
Format: Valid email address
Example: "sarah.chen@company.com"
Validation: Must pass email verification
Source: Lead list, company website
```

#### Company

```
Variable: {{company}}
Format: Text, proper case
Example: "Acme Corporation"
Note: Use official company name, not domain
Source: Lead list, LinkedIn
```

---

### Recommended Fields

#### Job Title

```
Variable: {{customField1}}
Format: Text
Example: "VP of Sales"
Usage: Role-based messaging, qualification
Source: LinkedIn, company website
```

#### LinkedIn URL

```
Variable: {{customField2}}
Format: Full URL
Example: "https://linkedin.com/in/sarahchen"
Usage: Research, verification
Source: Lead list, LinkedIn search
```

#### Icebreaker

```
Variable: {{customField3}}
Format: 1-2 sentences, AI-generated
Example: "Saw your post on scaling SDR teams — really resonated with 
the point about quality vs. quantity."
Usage: Personalized opening line
Source: AI-generated from research data
```

---

### Optional Enrichment Fields

#### Company Size

```
Variable: {{customField4}}
Format: Number or range
Example: "150" or "100-200"
Usage: Segmentation, qualification
Source: LinkedIn, Apollo, Clearbit
```

#### Industry

```
Variable: {{customField5}}
Format: Text
Example: "B2B SaaS"
Usage: Industry-specific messaging
Source: LinkedIn, company website
```

#### Pain Point

```
Variable: {{customField6}}
Format: Short phrase
Example: "scaling outbound without losing quality"
Usage: Relevance in email body
Source: AI-inferred from role/industry
```

#### Trigger Event

```
Variable: {{customField7}}
Format: Brief description
Example: "Just raised Series B"
Usage: Timely, relevant hook
Source: Crunchbase, Google News, LinkedIn
```

#### Tech Stack

```
Variable: {{customField8}}
Format: Comma-separated list
Example: "Salesforce, Outreach, Gong"
Usage: Solution fit, relevance
Source: BuiltWith, Wappalyzer, job postings
```

#### Recent News/Activity

```
Variable: {{customField9}}
Format: Brief summary
Example: "Published article on sales automation last week"
Usage: Personalization hook
Source: LinkedIn, Google News, company blog
```

#### Case Study Match

```
Variable: {{customField10}}
Format: Company name or snippet
Example: "TechCorp (similar industry, saw 3x meetings)"
Usage: Relevant social proof
Source: Internal case study matching
```

---

## Sample Lead Record

```csv
firstName,lastName,email,company,customField1,customField2,customField3,customField4,customField5,customField6,customField7
Sarah,Chen,sarah@techcorp.com,TechCorp,VP of Sales,https://linkedin.com/in/sarahchen,"Saw you're hiring 5 SDRs — scaling outbound is exciting but tricky",250,B2B SaaS,scaling outbound quality,Series B announced
```

---

## Data Quality Requirements

### Before Import

- [ ] All emails verified (use verification service)
- [ ] No duplicate emails
- [ ] Company names standardized (not domains)
- [ ] Job titles cleaned (consistent formatting)
- [ ] Required fields populated for all records

### Quality Thresholds

| Metric | Acceptable | Target |
|--------|------------|--------|
| Email validity | >95% | >98% |
| Required fields populated | 100% | 100% |
| Icebreaker populated | >80% | >95% |
| Company size populated | >70% | >90% |

---

## Fallback Handling

When fields are empty, use fallbacks in Smartlead:

### Spintax Fallback Syntax

```
{{{customField3}}|Noticed {{company}} has been growing fast lately}
```

If `customField3` (icebreaker) is empty, uses the generic fallback.

### Recommended Fallbacks

| Field | Fallback |
|-------|----------|
| First Name | "there" or "Hi," (no name) |
| Icebreaker | Generic company/industry reference |
| Pain Point | Common pain for their role |
| Trigger Event | Omit from email |

---

## Data Sources

### Primary Sources

| Source | Fields | Cost |
|--------|--------|------|
| LinkedIn Sales Navigator | Name, title, company, activity | Paid |
| Apollo.io | All contact fields, enrichment | Paid/Free tier |
| Clearbit | Company data, tech stack | Paid |
| Hunter.io | Email verification | Paid/Free tier |

### Enrichment Sources

| Source | Data | Cost |
|--------|------|------|
| BuiltWith | Tech stack | Paid |
| Crunchbase | Funding, news | Paid/Free |
| Google News | Recent news | Free |
| Company website | About page, blog | Free |

---

## Import Checklist

Before importing to Smartlead:

- [ ] CSV properly formatted (UTF-8, comma-delimited)
- [ ] Column headers match Smartlead field names
- [ ] Email column verified
- [ ] No special characters breaking fields
- [ ] Test import with 10 records first
- [ ] Custom fields mapped correctly

---

## Sample CSV Template

```csv
firstName,lastName,email,company,customField1,customField2,customField3,customField4,customField5
[First Name],[Last Name],[Email],[Company Name],[Job Title],[LinkedIn URL],[Icebreaker],[Company Size],[Industry]
```

Download and use this as your import template.

---

*Last updated: [Date]*
