# kanye.rest (kanye-rest)

Free single-purpose REST API that returns random Kanye West quotes, dubbed "Kanye as a Service." Hosted on Cloudflare Workers, the API exposes a JSON endpoint, a plain-text endpoint, and a full-quotes-array endpoint. The underlying project is open source (MIT) under github.com/ajzbc/kanye.rest and is a popular example of a minimal "fun" public API.

**URL:** [Visit APIs.json URL](https://kanye.rest)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Personality, Quotes, Open Source, Cloudflare Workers, Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## APIs

### kanye.rest

The Kanye REST API returns random Kanye West quotes. Three operations are exposed: a JSON quote endpoint at the root, a plain-text endpoint at /text, and a full-collection endpoint at /quotes returning all quotes as a JSON array. All endpoints are unauthenticated GETs with permissive CORS.

**Human URL:** [https://kanye.rest](https://kanye.rest)

#### Tags:

 - Personality, Quotes

#### Properties

- [Documentation](https://kanye.rest)
- [SourceCode](https://github.com/ajzbc/kanye.rest)
- [OpenAPI](openapi/kanye-rest-openapi.yml)
- [NaftikoCapability](capabilities/kanye-rest-quotes.yaml)

## Common Properties

- [Website](https://kanye.rest)
- [SourceCode](https://github.com/ajzbc/kanye.rest)
- [License — MIT License](https://github.com/ajzbc/kanye.rest/blob/master/LICENSE)
- [CLI — kanye.rest-cli (archived)](https://github.com/ajzbc/kanye.rest-cli)
- [PublicAPIsListing](https://github.com/public-apis/public-apis)
- [SpectralRules](rules/kanye-rest-spectral-rules.yml)
- [Vocabulary](vocabulary/kanye-rest-vocabulary.yml)
- [JSONLD](json-ld/kanye-rest-context.jsonld)
- [JSONSchema — Quote](json-schema/kanye-rest-quote-schema.json)
- [JSONSchema — QuoteList](json-schema/kanye-rest-quote-list-schema.json)
- [JSONStructure — Quote](json-structure/kanye-rest-quote-structure.json)
- [JSONStructure — QuoteList](json-structure/kanye-rest-quote-list-structure.json)
- [Example — Quote Example](examples/kanye-rest-quote-example.json)
- [Example — QuoteList Example](examples/kanye-rest-quote-list-example.json)
- [RateLimits](rate-limits/kanye-rest-rate-limits.yml)

## Features

| Name | Description |
|------|-------------|
| Random Quote (JSON) | Returns a single random Kanye West quote wrapped in a JSON object. |
| Random Quote (Plain Text) | Returns a single random Kanye West quote as plain text, useful for shell pipelines. |
| Full Quote Collection | Returns the complete array of available Kanye West quotes as JSON. |
| No Authentication | All endpoints are publicly accessible with no API key or token required. |
| CORS-Enabled | Responses include Access-Control-Allow-Origin "*" so the API is callable from any browser. |
| Edge-Hosted | Deployed on Cloudflare Workers, delivering responses from the global edge network. |

## Use Cases

| Name | Description |
|------|-------------|
| Hello-World API Demo | Used widely in tutorials and bootcamp curricula as a zero-friction example of consuming a REST API. |
| Frontend Component Testing | Lightweight fixture for testing fetch / loading / error states in UI frameworks without bringing up a backend. |
| Shell One-Liners | The /text endpoint produces shell-friendly output for cron jobs, daily-quote scripts, and motd files. |
| Bot and Chatbot Integrations | Plain-text quotes are easily injected into Slack, Discord, and Twitter bots. |

## Integrations

| Name | Description |
|------|-------------|
| Cloudflare Workers | API runtime — every request is served from a Cloudflare Worker at the edge. |
| GitHub | Source of truth for the open source implementation and release history. |

## Solutions

| Name | Description |
|------|-------------|
| Public-APIs Catalog Entry | Registered in the community-maintained public-apis directory under the Personality category. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Kanye REST OpenAPI](openapi/kanye-rest-openapi.yml) — 3 operations (`GET /`, `GET /text`, `GET /quotes`) under one tag (Quotes), with named examples and Microcks dispatcher extensions.

### JSON Schema

- [Quote](json-schema/kanye-rest-quote-schema.json)
- [QuoteList](json-schema/kanye-rest-quote-list-schema.json)

### JSON Structure

- [Quote](json-structure/kanye-rest-quote-structure.json)
- [QuoteList](json-structure/kanye-rest-quote-list-structure.json)

### JSON-LD

- [kanye-rest-context.jsonld](json-ld/kanye-rest-context.jsonld) — 5 terms mapping Quote / QuoteList and aligning `quote`, `name`, `description`, `url` to schema.org.

### Examples

- [Quote example](examples/kanye-rest-quote-example.json)
- [QuoteList example](examples/kanye-rest-quote-list-example.json)

## Capabilities

Naftiko capabilities exposing the Kanye REST endpoints over both a Spectral-compliant REST surface and an MCP tool surface.

### kanye.rest

- [Kanye REST — Quotes](capabilities/kanye-rest-quotes.yaml) — 3 consumed operations, 3 REST resources, 3 MCP tools.

## Rate Limits

- [Kanye REST Rate Limits](rate-limits/kanye-rest-rate-limits.yml) — Provider does not publish per-key or per-account request-rate numbers. Captures Cloudflare Workers platform-level caps and best-effort backoff guidance.

## Vocabulary

- [Kanye REST Vocabulary](vocabulary/kanye-rest-vocabulary.yml) — Unified taxonomy mapping 1 resource, 2 actions, 1 workflow, and 3 personas across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [Kanye REST Spectral Rules](rules/kanye-rest-spectral-rules.yml) — 40 rules across 12 categories enforcing Kanye REST conventions (OpenAPI 3.0.x, HTTPS edge host, camelCase operationIds, lowercase paths, Title Case summaries prefixed with "Kanye REST", no auth, no parameters, no request bodies).

## Source

This entry was bulk-registered as part of a public-apis catalog sweep on 2026-05-28, then enriched on 2026-05-29 with a full opensource pipeline pass (OpenAPI, JSON Schema, JSON Structure, JSON-LD, examples, Naftiko capability, Spectral rules, vocabulary, rate limits).

- **x-type:** opensource
- **x-tier:** 3 (bulk-registered from public-apis)
- **source:** [public-apis/public-apis](https://github.com/public-apis/public-apis) — category: Personality

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
