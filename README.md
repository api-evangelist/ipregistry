# IPregistry (ipregistry)

IPregistry provides a fast, reliable IP geolocation and threat intelligence REST API for looking up information associated with IPv4 or IPv6 addresses and Autonomous System Numbers (ASN). The API returns location data, connection details, company and carrier information, time zone, currency, and comprehensive security threat assessments drawn from over 220 OSINT threat feeds. It supports single and batch IP lookups (up to 1,024 IPs per request), user-agent parsing, ASN queries, and optional EU-region routing for GDPR-aligned data residency. All lookups are authenticated via API key and billed against prepaid credits that never expire. IPregistry is operated by Elaunira SARL, based in France.

APIs.json: https://raw.githubusercontent.com/api-evangelist/ipregistry/refs/heads/main/apis.yml

Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=ipregistry-api-evangelist&utm_content=repo

## Tags

- IP Geolocation
- Threat Intelligence
- IP Address
- ASN
- Carrier
- Security
- Location Data
- User-Agent Parsing
- VPN Detection
- Proxy Detection

## APIs

### IPregistry IP Geolocation and Threat Intelligence API

A REST API that resolves IPv4/IPv6 addresses and Autonomous System Numbers to rich intelligence including geolocation, ISP/carrier details, company data, currency and time zone, and threat classification across VPN, proxy, TOR, bot, and abuse categories. Supports single lookups, batch requests of up to 1,024 IPs, user-agent parsing, and ASN lookups, with an optional EU base URL for GDPR-aligned data routing.

- Base URL: https://api.ipregistry.co
- Documentation: https://ipregistry.co/docs

## Plans, Rate Limits, and FinOps

### Plans

IPregistry uses a prepaid credit model with no monthly fees and no credit expiration. New accounts receive 100,000 free credits on sign-up.

| Plan | Credits | Price | Per-Credit Cost |
|------|---------|-------|-----------------|
| Free Starter | 100,000 | $0 (one-time) | $0.0000 |
| Starter Pack | 50,000 | $10 | $0.0002 |
| Growth Pack | 400,000 | $50 | $0.000125 |
| Business Pack | 1,000,000 | $100 | $0.0001 |
| Scale Pack | 6,000,000 | $500 | ~$0.0000833 |
| Enterprise | Custom | Custom/month | Negotiated |

Full plan details: [plans/ipregistry-plans-pricing.yml](plans/ipregistry-plans-pricing.yml)

### Rate Limits

Rate limiting is not enforced by default. The account's credit balance is the primary constraint. Optional hourly invocation limits can be configured per API key in the dashboard. Batch requests are capped at 1,024 IPs, 16 ASNs, or 256 user-agent strings per request.

Full rate limit details: [rate-limits/ipregistry-rate-limits.yml](rate-limits/ipregistry-rate-limits.yml)

### FinOps

Each lookup costs 1 credit; batch requests cost (n + 1) credits. Cost per credit decreases with larger pack purchases. Spend controls include per-key hourly limits, low-balance alerts, and auto-renewal thresholds, all configurable from the dashboard.

Full FinOps details: [finops/ipregistry-finops.yml](finops/ipregistry-finops.yml)

## Timestamps

- Created: 2026-06-12
- Modified: 2026-06-12

## Common

| Type | URL |
|------|-----|
| Website | https://ipregistry.co |
| Documentation | https://ipregistry.co/docs |
| GitHub Org | https://github.com/ipregistry |
| LinkedIn | https://www.linkedin.com/company/ipregistry |
| Blog | https://ipregistry.co/blog |
| Pricing | https://ipregistry.co/pricing |
| Status Page | https://ipregistry.co/status |
| X (Twitter) | https://twitter.com/ipregistryco |
| Changelog | https://ipregistry.co/changelog |

## Maintainers

- Kin Lane — kin@apievangelist.com
