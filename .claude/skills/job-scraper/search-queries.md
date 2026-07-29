# Search Queries for Job Scraper

<!-- Configured for: Javier Montalvo - Senior Full Stack Developer, fully-remote (global) -->

## Search Sites

The built-in portal CLIs are Denmark-specific and are NOT used. Javier targets fully-remote
international roles, so search LinkedIn plus global remote job boards and company career pages.

Primary:
- **linkedin.com/jobs** - filter by "Remote"; keywords below
- **remoteok.com** - remote-first tech roles
- **weworkremotely.com** - remote developer roles
- **wellfound.com** (AngelList) - startup remote roles

Secondary (company career pages via Google):
- Direct Google searches with `site:` filters for known target companies
- General remote-board searches with `"remote"` in the query

## Query Categories

Queries are grouped by priority. All roles are fully remote, so combine each query with
`remote` (and optionally `LatAm` or `Americas timezone`) rather than a city.

### Priority 1: Senior Full Stack Developer

Strongest and most desired direction.

```
site:linkedin.com/jobs "Senior Full Stack Developer" remote
site:linkedin.com/jobs "Full Stack Engineer" React Node remote
site:remoteok.com "full stack" react node
"Senior Full Stack" (React OR Next.js) (Node OR Python) remote
```

### Priority 2: Tech Lead (hands-on)

Hands-on technical leadership without leaving the code.

```
site:linkedin.com/jobs "Tech Lead" React remote
site:linkedin.com/jobs "Engineering Lead" (hands-on OR "player coach") remote
"Technical Lead" full stack remote (Americas OR LatAm)
```

### Priority 3: Frontend Engineer (React / Vue / Next.js)

```
site:linkedin.com/jobs "Senior Frontend Engineer" (React OR Vue OR Next.js) remote
site:remoteok.com frontend react
site:weworkremotely.com "front end" (react OR vue) remote
```

### Priority 4: AI Automation / AI Engineer

Adjacent direction leveraging OpenAI/LLM and n8n experience.

```
site:linkedin.com/jobs "AI Engineer" (OpenAI OR LLM) remote
site:linkedin.com/jobs "AI Automation" (n8n OR OpenAI) remote
"AI Engineer" (full stack OR TypeScript) remote (Americas OR LatAm)
```

## Location Filter

Javier is based in Quito, Ecuador and requires fully-remote work. When evaluating results:
- **PASS:** fully remote worldwide, or remote within the Americas / US timezone overlap
- **PASS:** remote-first with occasional optional travel
- **FAIL:** on-site or hybrid requiring presence outside Quito
- **FLAG:** local-currency-only pay well below competitive international/USD rates

There is no commute radius to enforce - the filter is remote-eligibility and timezone overlap.

## Date Filter

Only include jobs posted within the last 14 days, or with an application deadline that has not
yet passed. If a posting date cannot be determined, include it but flag as "date unknown".

## Adapting Queries

If the user specifies a focus area, select queries from the matching category and also generate
2-3 custom queries for that focus. For example:
- "/scrape ai" -> Priority 4 queries + custom AI/LLM-specific queries
- "/scrape frontend" -> Priority 3 queries + custom React/Vue-specific queries
