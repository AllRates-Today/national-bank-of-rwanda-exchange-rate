# National Bank of Rwanda Exchange Rates API — national-bank-of-rwanda-exchange-rate

[![npm version](https://img.shields.io/npm/v/national-bank-of-rwanda-exchange-rate.svg)](https://www.npmjs.com/package/national-bank-of-rwanda-exchange-rate)
[![license](https://img.shields.io/npm/l/national-bank-of-rwanda-exchange-rate.svg)](https://github.com/AllRates-Today/national-bank-of-rwanda-exchange-rate/blob/main/LICENSE)
[![zero dependencies](https://img.shields.io/badge/dependencies-0-brightgreen.svg)](https://www.npmjs.com/package/national-bank-of-rwanda-exchange-rate)
[![TypeScript](https://img.shields.io/badge/TypeScript-types%20included-3178C6.svg)](https://www.typescriptlang.org/)
[![USD/RWF today](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Fbnrw%3Fsource%3DUSD%26target%3DRWF&query=%24.rate&label=USD%2FRWF%20published%20by%20National%20Bank%20of%20Rwanda&color=0A7E8C&cacheSeconds=3600)](https://allratestoday.com/central-bank-rates-api/bnrw/)
[![rate date](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Fbnrw%3Fsource%3DUSD%26target%3DRWF&query=%24.rate_date&label=rate%20date&color=555&cacheSeconds=3600)](https://allratestoday.com/central-bank-rates-api/bnrw/)

**Official National Bank of Rwanda (Rwanda) daily exchange rates for Node.js and TypeScript. The published central bank rates behind tax filings, customs valuations, audits, and compliant invoicing — not market estimates, but the numbers National Bank of Rwanda itself prints, every business day.**

## 🚀 Why this client?

- 🏛️ **Official published rates** — National Bank of Rwanda's own table, with the publisher's own `rate_date` on every response
- 📅 **History back to 2012** — point-in-time tables and daily series for any past date
- 🔀 **Published vs derived, always flagged** — computed inverse/cross pairs carry `derived: true`, never mixed with official prints
- ⚡ **Zero dependencies** — pure ESM + CJS over global `fetch`; Node 18+, Bun, Deno, and edge runtimes
- 🔷 **Type-safe** — full TypeScript definitions shipped with the package
- 🧾 **Compliance-grade metadata** — `rate_type`, publication date, and source disclaimer on every response

> **Official rate, not mid-market:** every value here is a number National Bank of Rwanda itself published, fixed once printed and carrying the central bank's own `rate_date` — what filings and audits require. Need the live mid-market rate for pricing or display instead? Use the [mid-market API](https://allratestoday.com/docs/) or [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk). The two can diverge by several percent.

## 🔑 Get your API key

Get a free API key at [allratestoday.com/register](https://allratestoday.com/register) — no credit card required. Latest rates are on every plan, including free.

## 📈 Latest published table

[![Latest National Bank of Rwanda table](https://allratestoday.com/api/open/central-bank/bnrw/table.svg)](https://allratestoday.com/central-bank-rates-api/bnrw/)

The image is rendered live from the keyless endpoint, so it follows the central bank's publications on npm and on GitHub alike without a new release. The same table as text is folded below for search and copy-paste: on GitHub [a daily Action](.github/workflows/daily-table.yml) refreshes it whenever the central bank publishes a new table; on npm it is as of the package's publish date.

<!-- daily-table:start -->
<details>
<summary>Table as text: published 2026-10-30 by National Bank of Rwanda — 60 rates. Updated 2026-10-30.</summary>

| Base | Quote | Type | Rate |
| --- | --- | --- | ---: |
| AED | RWF | buy | 400.580323 |
| AED | RWF | reference | 401.941721 |
| AED | RWF | sell | 403.303118 |
| AUD | RWF | buy | 1035.216916 |
| AUD | RWF | reference | 1038.735167 |
| AUD | RWF | sell | 1042.253417 |
| BIF | RWF | buy | 0.490649 |
| BIF | RWF | reference | 0.492316 |
| BIF | RWF | sell | 0.493984 |
| CAD | RWF | buy | 1052.781693 |
| CAD | RWF | reference | 1056.359638 |
| CAD | RWF | sell | 1059.937583 |
| CHF | RWF | buy | 1788.161598 |
| CHF | RWF | reference | 1794.238778 |
| CHF | RWF | sell | 1800.315958 |
| CNY | RWF | buy | 220.947053 |
| CNY | RWF | reference | 221.697956 |
| CNY | RWF | sell | 222.448858 |
| DKK | RWF | buy | 220.135681 |
| DKK | RWF | reference | 220.883826 |
| DKK | RWF | sell | 221.631971 |
| ETB | RWF | buy | 9.109732 |
| ETB | RWF | reference | 9.140692 |
| ETB | RWF | sell | 9.171652 |
| EUR | RWF | buy | 1647.7552 |
| EUR | RWF | reference | 1653.3552 |
| EUR | RWF | sell | 1658.9552 |
| GBP | RWF | buy | 1971.4214 |
| GBP | RWF | reference | 1978.1214 |
| GBP | RWF | sell | 1984.8214 |
| INR | RWF | buy | 15.443291 |
| INR | RWF | reference | 15.495776 |
| INR | RWF | sell | 15.548261 |
| JPY | RWF | buy | 9.330414 |
| JPY | RWF | reference | 9.362124 |
| JPY | RWF | sell | 9.393834 |
| KES | RWF | buy | 11.316547 |
| KES | RWF | reference | 11.355007 |
| KES | RWF | sell | 11.393467 |
| NOK | RWF | buy | 159.396041 |
| NOK | RWF | reference | 159.937758 |
| NOK | RWF | sell | 160.479476 |
| SAR | RWF | buy | 392.030386 |
| SAR | RWF | reference | 393.362726 |
| SAR | RWF | sell | 394.695066 |
| SEK | RWF | buy | 149.664722 |
| SEK | RWF | reference | 150.173367 |
| SEK | RWF | sell | 150.682012 |
| TZS | RWF | buy | 0.556117 |
| TZS | RWF | reference | 0.558007 |
| TZS | RWF | sell | 0.559897 |
| UGX | RWF | buy | 0.338378 |
| UGX | RWF | reference | 0.339528 |
| UGX | RWF | sell | 0.340678 |
| USD | RWF | buy | 1471.21 |
| USD | RWF | reference | 1476.21 |
| USD | RWF | sell | 1481.21 |
| ZAR | RWF | buy | 88.530797 |
| ZAR | RWF | reference | 88.831675 |
| ZAR | RWF | sell | 89.132552 |

</details>

Source: [Official rates published by BNRW, served by AllRatesToday](https://allratestoday.com/central-bank-rates-api/bnrw/). Rates are as printed by the central bank; AllRatesToday is not affiliated with it.
<!-- daily-table:end -->

## 📦 Installation

```bash
npm install national-bank-of-rwanda-exchange-rate
```

```bash
yarn add national-bank-of-rwanda-exchange-rate
```

```bash
pnpm add national-bank-of-rwanda-exchange-rate
```

Requires Node 18+ (global `fetch`); also runs on Bun, Deno and edge runtimes. Also published under the org scope as [`@allratestoday/national-bank-of-rwanda-exchange-rate`](https://www.npmjs.com/package/@allratestoday/national-bank-of-rwanda-exchange-rate) — same code, same versions.

## 🏁 Quick start

```js
import { getRate } from 'national-bank-of-rwanda-exchange-rate';

const pair = await getRate('USD', 'RWF', { apiKey: 'art_live_...' });
console.log(pair.rate, pair.rate_date); // the official National Bank of Rwanda rate, on the central bank's own date
```

## 📚 API reference

- [Latest pair rate](#latest-pair-rate) — one pair from the latest published table
- [Full published table](#full-published-table) — everything the central bank printed, in one call
- [Table for a date](#table-for-a-date) — the official table for an invoice or filing date
- [Daily time series](#daily-time-series) — one pair across a date range

---

### Latest pair rate

Free plan and up. Pairs the central bank does not print directly are resolved from its table and flagged (see *Published vs derived rates* below).

```js
const pair = await getRate('USD', 'RWF', { apiKey: 'art_live_...' });
```

**Response:**

```javascript
{
  bank: 'bnrw',
  name: 'National Bank of Rwanda',
  rate_date: '2026-10-14',   // National Bank of Rwanda's own publication date
  source: 'USD',
  target: 'RWF',
  rate: 1474.995,
  rate_type: 'reference',
  derived: false,
  method: 'published',
  disclaimer: 'Official rates as published by the named central bank. On weekends/holidays the most recent published rate_date is returned.'
}
```

### Full published table

Free plan and up. The complete table for the latest publication date.

```js
import { getLatestRates } from 'national-bank-of-rwanda-exchange-rate';

const table = await getLatestRates({ apiKey: 'art_live_...' });
console.log(table.rate_date, table.rates.length);
```

**Response:**

```javascript
{
  bank: 'bnrw',
  name: 'National Bank of Rwanda',
  rate_date: '2026-10-14',
  rates: [
    { "base": "USD", "quote": "RWF", "type": "reference", "value": 1474.995 },
    { "base": "USD", "quote": "RWF", "type": "sell", "value": 1479.995 },
    { "base": "USD", "quote": "RWF", "type": "buy", "value": 1469.995 },
    // … the rest of the published table (21 currencies vs RWF)
  ],
  disclaimer: '…'
}
```

### Table for a date

Paid plans. The official table for any date since 2012 — weekends and holidays return the most recent published date, flagged via `published_on_requested_date`, which is exactly the in-force rate a filing needs.

```js
import { getRatesForDate } from 'national-bank-of-rwanda-exchange-rate';

const day = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...' });
// Optionally narrow to one pair:
const one = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...', source: 'USD', target: 'RWF' });
```

**Response:**

```javascript
{
  bank: 'bnrw',
  requested_date: '2026-06-30',
  rate_date: '2026-06-30',                // the date actually published
  published_on_requested_date: true,      // false when a weekend/holiday fell back
  rates: [ /* the full table for that date */ ],
  disclaimer: '…'
}
```

### Daily time series

Paid plans. One resolved rate per publication date — ready for charting, revaluation runs, or audit workpapers.

```js
import { getHistory } from 'national-bank-of-rwanda-exchange-rate';

const series = await getHistory(
  { source: 'USD', target: 'RWF', from: '2026-01-01', to: '2026-10-14' },
  { apiKey: 'art_live_...' }
);
```

**Response:**

```javascript
{
  bank: 'bnrw',
  source: 'USD',
  target: 'RWF',
  from: '2026-01-01',
  to: '2026-10-14',
  count: 152,
  rates: [
    // one entry per publication date
    { date: '2026-10-14', rate: 1474.995, rate_type: 'reference', derived: false, method: 'published' },
    // …
  ],
  disclaimer: '…'
}
```

Pass `{ symbol: 'USD' }` instead of `source`/`target` to get the raw published rows for one currency (all rate types, no pair resolution).

---

## 🗺️ Currencies covered

National Bank of Rwanda currently publishes rates covering **21 currencies** against the RWF (as of the latest table):

🇦🇪 `AED` · 🇦🇺 `AUD` · 🇧🇮 `BIF` · 🇨🇦 `CAD` · 🇨🇩 `CDF` · 🇨🇭 `CHF` · 🇨🇳 `CNY` · 🇩🇰 `DKK` · 🇪🇹 `ETB` · 🇪🇺 `EUR` · 🇬🇧 `GBP` · 🇮🇳 `INR` · 🇯🇵 `JPY` · 🇰🇪 `KES` · 🇳🇴 `NOK` · 🇸🇦 `SAR` · 🇸🇪 `SEK` · 🇹🇿 `TZS` · 🇺🇬 `UGX` · 🇺🇸 `USD` · 🇿🇦 `ZAR`

## 🏛️ Source

The National Bank of Rwanda publishes daily official franc rates — an average (reference) rate with buying and selling quotes — for the major world and East African currencies. Kigali's rate matters well beyond Rwanda's borders: the franc corridor with Kenya, Tanzania and Uganda carries substantial regional trade, and the series reaches back to 2012.

- Publisher's own page: [Exchange rates](https://www.bnr.rw/exchange-rate/) · [www.bnr.rw](https://www.bnr.rw)
- Publication: every business day; the exact schedule, freshness status and any current delay are on the [National Bank of Rwanda rates page](https://allratestoday.com/central-bank-rates-api/bnrw/)
- In the API: usually by **08:20 UTC** (measured over the last 11 publications). Schedule a sync at or after that time and retry hourly until `rate_date` moves; every response carries the same figure as `available_by_utc` — see [when to poll](https://allratestoday.com/docs/#when-to-poll)
- Values are stored unmodified, with the publisher's own `rate_date` on every row — see the [methodology](https://allratestoday.com/official-rates-methodology/)

## 🧭 Reading the numbers

- `value` is always **quote currency per 1 unit of base currency** (`base: "EUR", quote: "USD", value: 1.15` means 1 EUR = 1.15 USD).
- National Bank of Rwanda quotes **RWF per 1 unit of foreign currency** (e.g. `base: "USD", quote: "RWF"` means RWF per one US dollar).
- Need the other way round? Ask `getRate(target, source)` and the API inverts or crosses for you, flagged `derived: true` — never divide a published rate yourself in a compliance workflow.
- `rate_type` tells you which of the central bank's series a row belongs to (`reference` here); some publishers print buy/sell or several fixings for the same pair.

## 🧩 ERP & accounting systems

Loading the official National Bank of Rwanda rate into an accounting system is a supported workflow, not a hack. Step-by-step guides with the direction each system expects:

- [Dynamics 365 Business Central](https://allratestoday.com/docs/integrations/business-central/) — built-in Currency Exchange Rate Service, no code
- [Xero](https://allratestoday.com/docs/integrations/xero/) · [QuickBooks Online](https://allratestoday.com/docs/integrations/quickbooks/) · [SAP S/4HANA and ECC](https://allratestoday.com/docs/integrations/sap/) · [Odoo](https://allratestoday.com/docs/integrations/odoo/)

The same keyed endpoints return `?format=csv`, `?format=xml` and `?format=xlsx`, and accept the key as `?api_key=` on the URL for importers that cannot send headers:

```bash
curl "https://allratestoday.com/api/v1/central-bank/bnrw/latest?format=xml&api_key=art_live_..."
```

## 🤖 AI agents

- MCP server: `npx -y @allratestoday/central-bank-mcp` (stdio) or the hosted endpoint `https://allratestoday.com/api/mcp` — tools for official rates, history, cross-bank comparison and publication calendars
- Already using the general SDK or MCP server? Since 2026-10-01 [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk) 1.4+ has `officialRates('bnrw')` and [`@allratestoday/mcp-server`](https://www.npmjs.com/package/@allratestoday/mcp-server) 0.6+ has a `get_official_rates` tool — both return this source's latest table with no key, so you can add it without a second dependency
- Claude Code plugin (no key): `/plugin marketplace add AllRates-Today/claude-code-plugin` then `/plugin install allratestoday@allratestoday` — bundles both MCP servers plus an `/official-rate bnrw ...` command
- Evaluating? Agents can self-issue a trial key with no signup: `POST https://allratestoday.com/api/agent/keys` (send `Content-Type: application/json`) returns a 100-call key valid 7 days that covers the free-plan methods (latest table, pairs); dated tables and history need a [paid plan](https://allratestoday.com/pricing/). The MCP servers expose it as `request_trial_key`
- Machine-readable site guide: [llms.txt](https://allratestoday.com/llms.txt) · [for-ai-agents](https://allratestoday.com/for-ai-agents/)

## ⚖️ Published vs derived rates

If National Bank of Rwanda does not print a pair directly, the API resolves it from the central bank's own table and says so — official and computed values are never confused:

| `method` | `derived` | Meaning |
| --- | --- | --- |
| `published` | `false` | The central bank printed this pair directly |
| `inverse` | `true` | Computed as 1 ÷ the published opposite direction |
| `cross` | `true` | Computed via RWF from two published rates |

## 🛡️ Error handling

Errors are thrown as `Error` with `status` (HTTP code) and `body` (the API's JSON error) attached:

```js
try {
  const pair = await getRate('USD', 'XXX', { apiKey: 'art_live_...' });
} catch (err) {
  console.log(err.message); // human-readable reason
  console.log(err.status);  // e.g. 404
}
```

| Status | Meaning |
| ------ | ------- |
| — | Missing `apiKey` (thrown before any request) |
| `400` | Malformed date or parameters |
| `401` | Invalid API key |
| `403` | Endpoint needs a [paid plan](https://allratestoday.com/pricing/) (historical dates & series) |
| `404` | Pair or date range not covered by National Bank of Rwanda |
| `429` | Monthly quota exceeded |

## 🔷 TypeScript

Full definitions ship with the package — no `@types` install:

```ts
import type { LatestRates, PairRate, DatedRates, RateEntry, HistoryQuery, RequestOptions } from 'national-bank-of-rwanda-exchange-rate';
```

## 📦 CommonJS

```javascript
const { getRate } = require('national-bank-of-rwanda-exchange-rate');

getRate('USD', 'RWF', { apiKey: 'art_live_...' }).then((pair) => console.log(pair.rate));
```

## 💡 Quota tips

- Rates change once per business day — cache the published table locally and a small monthly quota goes a long way.
- Every request counts toward your AllRatesToday quota, shared across all AllRatesToday endpoints on your key.

## 📖 Methods reference

| Method | Plan | Description |
| ------ | ---- | ----------- |
| `getRate(source, target, { apiKey })` | Free | Latest rate for one pair, resolved from the published table |
| `getLatestRates({ apiKey })` | Free | The central bank's full latest published table |
| `getRatesForDate(date, { apiKey, source?, target? })` | Paid | The official table (or one pair) for a YYYY-MM-DD date |
| `getHistory({ symbol \| source+target, from?, to? }, { apiKey })` | Paid | Daily series since 2012 |

## 📥 Bulk data (no key)

Need the whole archive rather than an API call? The same published tables are mirrored daily as open data:

- Hugging Face: [AllRatesToday/central-bank-exchange-rates](https://huggingface.co/datasets/AllRatesToday/central-bank-exchange-rates) — one CSV per institution (`rates/bnrw.csv`)
- Kaggle: [allratestoday/central-bank-exchange-rates](https://www.kaggle.com/datasets/allratestoday/central-bank-exchange-rates)
- Raw JSON on GitHub: `https://raw.githubusercontent.com/AllRates-Today/central-bank-exchange-rates/main/data/bnrw/latest.json`

## 🔗 Links

- [National Bank of Rwanda rates page](https://allratestoday.com/central-bank-rates-api/bnrw/) — live table, publication cadence, FAQ
- [All central bank sources](https://allratestoday.com/central-bank-rates-api/)
- [Package docs on the site](https://allratestoday.com/docs/sdk/national-bank-of-rwanda-exchange-rate/) · [ERP integration guides](https://allratestoday.com/docs/integrations/)
- [API documentation](https://allratestoday.com/docs/#central-bank) · [Interactive reference](https://allratestoday.com/api-reference/) · [Methodology](https://allratestoday.com/official-rates-methodology/)
- [Register (Free)](https://allratestoday.com/register) · [Dashboard](https://allratestoday.com/profile) · [Pricing](https://allratestoday.com/pricing/)
- [Status](https://allratestoday.com/status)
- [Postman collection](https://allratestoday.com/postman/)
- [GitHub](https://github.com/AllRates-Today/national-bank-of-rwanda-exchange-rate)

## 📜 License

MIT
