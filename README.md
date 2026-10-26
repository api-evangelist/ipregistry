# IPregistry (ipregistry)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
