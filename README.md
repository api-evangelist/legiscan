# LegiScan (legiscan)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

LegiScan is a national legislative tracking service providing real-time data on bill activity, voting records, and legislative actions across all 50 US states and Congress. The LegiScan API offers a JSON-based RPC-style interface supporting both pull and push data delivery models. Developers and organizations can monitor legislation in near real-time, search full-text bill content, retrieve roll call votes, access sponsor and legislator information, and download bulk session datasets. The free public tier provides 30,000 queries per month, with paid subscription plans offering higher limits and push-based real-time updates pushed every 15 minutes to 4 hours as changes are detected.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/legiscan/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/legiscan/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Legislative Tracking
- Government
- Bills
- Voting Records
- State Legislation
- Congressional Data
- Civic Tech

## Timestamps

- **Created:** 2026-06-13
- **Modified:** 2026-06-13

## APIs

### LegiScan Pull API

The LegiScan Pull API is an RPC-style JSON service that allows clients to query the national legislative database on demand. Operations include retrieving session lists, master bill lists, bill details, full bill text, amendments, supplements, roll call votes, person/sponsor information, and full-text search across all 50 states and Congress. Authentication uses an API key passed as a query parameter. The free public tier supports 30,000 queries per month; paid subscription tiers provide higher query limits.

- **Human URL:** [https://legiscan.com/legiscan](https://legiscan.com/legiscan)
- **Base URL:** `https://api.legiscan.com/`

#### Tags

- Bills
- Sessions
- Voting Records
- Legislators
- Search
- Amendments

#### Properties

- [Documentation](https://legiscan.com/legiscan)
- [API Reference](https://legiscan.com/gaits/documentation/legiscan)

### LegiScan Push API

The LegiScan Push API is a paid subscription service that delivers real-time legislative updates to a client-hosted endpoint. Changes detected in bill information are pushed every 15 minutes to 4 hours depending on subscription tier and coverage (single state to full national). Clients implement a push endpoint listener that validates incoming payloads via an Authorization header using the api_auth_key.

- **Human URL:** [https://legiscan.com/legiscan](https://legiscan.com/legiscan)
- **Base URL:** `https://api.legiscan.com/`

#### Tags

- Push Notifications
- Real-Time
- Webhooks
- Bills
- Legislation

#### Properties

- [Documentation](https://legiscan.com/legiscan)
- [API Reference](https://api.legiscan.com/docs/class-LegiScan_Endpoint.html)

### LegiScan Bulk Dataset API

The LegiScan Bulk Dataset API provides access to weekly snapshot ZIP archives containing all getBill, getRollCall, and getPerson payload records as individual JSON files for each legislative session. Clients retrieve dataset listings via getDatasetList and download archives via getDataset using a session_id and access_key. Datasets are available for all 50 states and Congress going back multiple sessions.

- **Human URL:** [https://legiscan.com/datasets](https://legiscan.com/datasets)
- **Base URL:** `https://api.legiscan.com/`

#### Tags

- Bulk Data
- Datasets
- Bills
- Sessions
- Archives

#### Properties

- [Documentation](https://legiscan.com/datasets)
- [Data Exports](https://legiscan.com/data-exports)

## Common Properties

- [Website](https://legiscan.com)
- [Documentation](https://legiscan.com/legiscan)
- [API Reference](https://legiscan.com/gaits/documentation/legiscan)
- [Blog](https://legiscan.com/news-update)
- [Pricing](https://legiscan.com/pricing/api)
- [LinkedIn](https://www.linkedin.com/company/legiscan)
- [X (Twitter)](https://x.com/LegiScan)
- [Plans](plans/legiscan-plans-pricing.yml)
- [Rate Limits](rate-limits/legiscan-rate-limits.yml)
- [Fin Ops](finops/legiscan-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
