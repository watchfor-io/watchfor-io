# WatchFor

**Uptime, API & synthetic monitoring** — for humans *and* AI agents.

<a href="https://ora.ai/scan/watchfor.io"><img src="https://ora.ai/api/badge/watchfor.io" alt="ora agent-readiness score" height="76" /></a> <a href="https://is-agentic.com/scan/watchfor.io"><img src="https://watchfor.io/api/badge/is-agentic" alt="is-agentic agent readiness score" height="76" /></a> <a href="https://webmcp.ora.ai/watchfor.io"><img src="https://watchfor.io/api/badge/webmcp" alt="WebMCP audit score" height="76" /></a>

[watchfor.io](https://watchfor.io) monitors websites, APIs, SSL certificates, DNS, email delivery and mailboxes, cron jobs, MCP servers, scripted browser journeys and Linux servers from 20 locations across 7 world regions. A failure is only declared **Down** once confirmed from several locations — alerts reflect real outages, not one bad network path.

## What WatchFor does

- **30 monitor types** — [HTTP/HTTPS](https://watchfor.io/http-monitoring) · [API with JSON assertions](https://watchfor.io/api-monitoring) · [Playwright browser checks](https://watchfor.io/playwright-monitoring) · [SSL certificates](https://watchfor.io/ssl-monitoring) · [DNS](https://watchfor.io/dns-monitoring) · [CDN caching](https://watchfor.io/cdn-monitoring) · [TCP](https://watchfor.io/tcp-monitoring) / [UDP](https://watchfor.io/udp-monitoring) · [ping/ICMP](https://watchfor.io/ping-monitoring) · [MTR network path](https://watchfor.io/mtr-monitoring) · [email deliverability](https://watchfor.io/email-monitoring) · [IMAP](https://watchfor.io/imap-monitoring) / [POP3](https://watchfor.io/pop3-monitoring) mailboxes and quota · [email round-trip](https://watchfor.io/email-round-trip-monitoring) · [cron jobs / heartbeats](https://watchfor.io/cron-job-monitoring) · [Core Web Vitals](https://watchfor.io/core-web-vitals-monitoring) · [MCP servers](https://watchfor.io/mcp-monitoring) · [page integrity / defacement](https://watchfor.io/page-integrity-monitoring) · [domain expiry](https://watchfor.io/domain-expiry-monitoring) · [blacklists](https://watchfor.io/blacklist-monitoring) and more
- **[Synthetic monitoring](https://watchfor.io/synthetic-monitoring)** — scripted checks that act like a user, on a schedule, from many locations: API checks, Core Web Vitals audits and browser checks, with an incident only once a failure is confirmed
- **[Browser checks](https://watchfor.io/playwright-monitoring)** — plain Playwright Test scripts (login, search, checkout) run on a schedule in a sandboxed Chromium: every step timed with a screenshot, secrets masked in results and traces, a test run before you save
- **Credentials stay secret** — the passwords, tokens and API-key headers you give a check are stored encrypted, never shown again (not even to owners) and only sent where they were entered; share one across checks as an org secret with `{{NAME}}` ([docs](https://watchfor.io/docs/monitors/web#credentials-and-variables))
- **[Server monitoring](https://watchfor.io/server-monitoring)** — the inside view next to the outside one: the open-source [watchfor-agent](https://github.com/watchfor-io/agent) pushes CPU, load, memory, disk, network and process metrics from Linux servers, with the same alerting as monitors
- **[CDN monitoring](https://watchfor.io/cdn-monitoring)** — is your edge really caching, or quietly hitting your origin? Cache hit ratio, which edge answers in each region, per-region performance, and an alert when caching breaks
- **Confirmed multi-location alerting** to 16 channels — email, Slack, Discord, Telegram, Microsoft Teams, Google Chat, PagerDuty, Opsgenie, ntfy, Zapier, webhooks… ([all integrations](https://watchfor.io/alerting-integrations))
- **[Public status pages](https://watchfor.io/status-pages)** on your own subdomain, with third-party components, badges and RSS
- **[Incident management](https://watchfor.io/incident-management)** — confirmed incidents, internal notes, post-mortems, maintenance windows that keep planned work out of your uptime
- **[On-call scheduling](https://watchfor.io/on-call)** — rotations and escalations, included in plans (no per-seat fees)
- **[Reports](https://watchfor.io/reporting)** — weekly/monthly email reports with MTTR/MTBF and trends, the same data over the API; custom periods and per-client (tag) reports on Pro and up
- **[Data history](https://watchfor.io/docs/organization/data-retention)** — uptime and incident history kept forever on every plan; charts up to 5 years, individual check results 30–180 days, screenshots, traces and Lighthouse reports 7–90 days

## For developers & agents

- 🔌 **REST API** — [watchfor.io/api/v1](https://watchfor.io/docs/api) · [OpenAPI 3.1](https://watchfor.io/openapi.json) (84 operations)
- 🤖 **MCP server** (59 tools) — `https://watchfor.io/api/mcp` · [Smithery](https://smithery.ai/servers/hello-65wl/watchfor)
- 📚 **Docs MCP server** (no auth) — `https://watchfor.io/api/docs-mcp`
- 🤝 **A2A agent** (18 skills) — `https://watchfor.io/api/a2a`
- 🧪 **No-auth sandbox** — `https://watchfor.io/api/v1/sandbox`
- 🩺 **Live diagnostics** (24 on-demand checks) — `https://watchfor.io/api/v1/diagnostics` · DNS, propagation, DNS health, TLS grade, mail server grade, HTTP headers, CDN, ping, traceroute, ports, e-mail policy and more, run from the probe fleet; graded checks return the same A+ to F grade as the dashboard, with what capped it and the fix. A model can reason about a site; it has no machine in 20 locations.
- 📈 **Prometheus metrics** (Pro plan and above) — `https://watchfor.io/api/v1/metrics` · status, incident-based uptime, response times, SSL and domain expiry, heartbeats and hosts for your own Prometheus, with a [Grafana dashboard](https://watchfor.io/docs/api/prometheus#grafana-dashboard)
- 🧭 **WebMCP (in-page tools)** — nine browser-side tools on `document.modelContext`, so an agent-capable browser can use watchfor.io with no account · [audit](https://webmcp.ora.ai/watchfor.io)

## SDKs & CLI

Official clients for the REST API — so a deploy script, a CI job or your own app can create monitors, read what is down, pull incidents and reports, or pause checks during a release without hand-writing HTTP calls. Zero dependencies, typed, resource for resource with the API, with idempotency keys for safe retries. The npm package also ships a `watchfor` CLI.

| Language | Install | Version |
| --- | --- | --- |
| TypeScript / JavaScript | [`npm install watchfor`](https://www.npmjs.com/package/watchfor) | [![npm](https://img.shields.io/npm/v/watchfor)](https://www.npmjs.com/package/watchfor) |
| Python | [`pip install watchfor`](https://pypi.org/project/watchfor/) | [![PyPI](https://img.shields.io/pypi/v/watchfor)](https://pypi.org/project/watchfor/) |
| Ruby | [`gem install watchfor`](https://rubygems.org/gems/watchfor) | [![Gem](https://img.shields.io/gem/v/watchfor)](https://rubygems.org/gems/watchfor) |

```ts
import { WatchFor } from "watchfor";

const wf = new WatchFor({ apiKey: process.env.WATCHFOR_API_KEY! });
const summary = await wf.summary();                        // what's up/down right now
const firing = await wf.incidents.list({ status: "firing" });
```

```bash
export WATCHFOR_API_KEY=wf_live_...
npx watchfor summary
npx watchfor incidents --status firing
npx watchfor report --period 30d
```

Docs: [watchfor.io/docs/api#sdks--cli](https://watchfor.io/docs/api#sdks--cli) · API key: dashboard → Settings → API keys

## Free tools — no signup

[62 free network, web and email tools](https://watchfor.io/free-tools), each with a [how-to guide](https://watchfor.io/blog/category/guides) built on a real run. The ones that need the internet's view run from our probe fleet in 20 locations — the same checks agents call as live diagnostics — so you see your site the way the world does, not the way your laptop does. The graded ones share **[WatchFor Grade](https://watchfor.io/grades)**: one A+ to F scale with published, versioned rules — start at A+, the worst finding sets the ceiling, every reason and fix is shown, and no grade when we couldn't measure:

- **[Smart Website Checker](https://watchfor.io/smart-website-audit)** — one scan, one letter grade with the reasons: domain expiry, HTTPS, DNS, email spoofing protection, mail blacklists
- **[Global CDN Checker](https://watchfor.io/cdn-checker)** — which CDN serves a URL, which edge answers in each region, whether it is really cached, and which regions behave differently; three requests from every location, one graded report
- **[SSL/TLS Grade](https://watchfor.io/ssl-grade-checker)** — A+ to F for protocols, ciphers, forward secrecy, post-quantum key exchange, HSTS and the certificate, with the exact reasons
- **[DNS Propagation](https://watchfor.io/dns-propagation-checker)** — a record as every region sees it, on a live world map: stale anycast nodes and propagation gaps
- **[DNS Health Checker](https://watchfor.io/dns-health-checker)** — nameservers, delegation, SOA, DNSSEC and CAA checked from several networks and graded A+ to F, each finding with its fix
- **[Core Web Vitals Checker](https://watchfor.io/core-web-vitals-checker)** — a full Lighthouse run: LCP, CLS, the loading filmstrip frame by frame, the top fixes and a performance grade
- **[MCP Server Checker](https://watchfor.io/mcp-server-checker)** — initialize handshake, protocol version, capabilities and the full tool inventory of any MCP server, graded for protocol, transport security, auth discovery and tool hygiene
- **[Mail Server Checker](https://watchfor.io/mail-server-checker)** — enter a domain and every mail server it uses (inbound MX, SMTP submission, IMAP, POP3) gets an A+ to F grade for TLS, certificates, STARTTLS, plain-text logins, open relay, MTA-STS, TLS-RPT and DANE, from three regions, with the exact fix; no login, no test message
- **[Email Health](https://watchfor.io/email-policy-checker)** — one SPF + DKIM + DMARC grade with per-record diagnostics, plus an [email header analyzer](https://watchfor.io/email-header-analyzer)

Also: [Ping](https://watchfor.io/ping-test) · [Traceroute](https://watchfor.io/traceroute-online) · [Port checker](https://watchfor.io/port-checker) · [Blacklist check](https://watchfor.io/blacklist-checker) · [Whois](https://watchfor.io/whois-lookup) · [DNS lookups](https://watchfor.io/dns-checker) (A, AAAA, CNAME, MX, NS, TXT, SOA, SRV, CAA, reverse) · [HTTP headers](https://watchfor.io/http-header-checker) · [Security headers](https://watchfor.io/security-headers-checker) (graded, with nginx / Apache / Caddy / Cloudflare fixes) · [Redirect checker](https://watchfor.io/redirect-checker) · [API tester](https://watchfor.io/api-tester) · [WebSocket tester](https://watchfor.io/websocket-tester) · [SMTP test](https://watchfor.io/smtp-test) · [What's my IP](https://watchfor.io/whats-my-ip) · calculators for [uptime](https://watchfor.io/uptime-calculator), [SLA](https://watchfor.io/sla-calculator), [error budget](https://watchfor.io/error-budget-calculator), [subnets](https://watchfor.io/subnet-calculator), [cron](https://watchfor.io/cron-expression-tester) and [JSON / JSONPath](https://watchfor.io/json-formatter)

## Open source

- **[`agent`](https://github.com/watchfor-io/agent)** — watchfor-agent, the Linux host agent [![release](https://img.shields.io/github/v/release/watchfor-io/agent?display_name=tag)](https://github.com/watchfor-io/agent/releases/latest) [![license](https://img.shields.io/github/license/watchfor-io/agent)](https://github.com/watchfor-io/agent/blob/main/LICENSE) — one static Go binary (amd64, arm64), a one-line install, outbound HTTPS only, nothing executed from configuration, signed and reproducible releases, opt-in auto-update · [about the agent](https://watchfor.io/agent)
- **[`prometheus-exporter`](https://github.com/watchfor-io/prometheus-exporter)** — polls the metrics endpoint for one or more organizations and serves it on `/metrics`: one target for several organizations, keys kept in a Kubernetes Secret, its own health metrics · Go, distroless image
- **[`agent-toolkit`](https://github.com/watchfor-io/agent-toolkit)** — AGENTS.md, agent skills, plugin manifest and MCP config

Agent quickstart: [watchfor.io/agents.md](https://watchfor.io/agents.md) · Docs: [watchfor.io/docs](https://watchfor.io/docs) · Comparisons: [watchfor.io/comparisons](https://watchfor.io/comparisons) · Engineering blog: [watchfor.io/blog](https://watchfor.io/blog) · Changelog: [watchfor.io/changelog](https://watchfor.io/changelog) · Press kit: [watchfor.io/press](https://watchfor.io/press)
