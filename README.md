# LegiScan (legiscan)

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
