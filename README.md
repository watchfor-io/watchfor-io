# WatchFor

**Uptime & infrastructure monitoring** — for humans *and* AI agents.

<a href="https://ora.ai/scan/watchfor.io"><img src="https://ora.ai/api/badge/watchfor.io" alt="ora agent-readiness score" height="76" /></a> <a href="https://is-agentic.com/scan/watchfor.io"><img src="https://watchfor.io/api/badge/is-agentic" alt="is-agentic agent readiness score" height="76" /></a> <a href="https://webmcp.ora.ai/watchfor.io"><img src="https://watchfor.io/api/badge/webmcp" alt="WebMCP audit score" height="76" /></a>

[watchfor.io](https://watchfor.io) monitors websites, APIs, SSL certificates, DNS, email, cron jobs and MCP servers from multiple regions worldwide. A failure is only declared **Down** once confirmed from several locations — alerts reflect real outages, not one bad network path.

## What WatchFor does

- **25 monitor types** — [HTTP/HTTPS](https://watchfor.io/http-monitoring) · [API with JSON assertions](https://watchfor.io/api-monitoring) · [SSL certificates](https://watchfor.io/ssl-monitoring) · [DNS](https://watchfor.io/dns-monitoring) · [TCP](https://watchfor.io/tcp-monitoring) / [UDP](https://watchfor.io/udp-monitoring) · [ping/ICMP](https://watchfor.io/ping-monitoring) · [MTR network path](https://watchfor.io/mtr-monitoring) · [email deliverability](https://watchfor.io/email-monitoring) · [cron jobs / heartbeats](https://watchfor.io/cron-job-monitoring) · [Core Web Vitals](https://watchfor.io/core-web-vitals-monitoring) · [MCP servers](https://watchfor.io/mcp-monitoring) · [domain expiry](https://watchfor.io/domain-expiry-monitoring) · [blacklists](https://watchfor.io/blacklist-monitoring) and more
- **Confirmed multi-location alerting** to 16+ channels — email, Slack, Discord, Telegram, Microsoft Teams, PagerDuty, Opsgenie, webhooks… ([all integrations](https://watchfor.io/alerting-integrations))
- **[Public status pages](https://watchfor.io/status-pages)** on your own subdomain, with third-party components, badges and RSS
- **[Incident management](https://watchfor.io/incident-management)** — timelines, internal notes, post-mortems
- **[On-call scheduling](https://watchfor.io/on-call)** — rotations and escalations, included in plans (no per-seat fees)

## For developers & agents

- 🔌 **REST API** — [watchfor.io/api/v1](https://watchfor.io/docs/api) · [OpenAPI 3.1](https://watchfor.io/openapi.json)
- 🤖 **MCP server** (45 tools) — `https://watchfor.io/api/mcp` · [Smithery](https://smithery.ai/servers/hello-65wl/watchfor)
- 📚 **Docs MCP server** (no auth) — `https://watchfor.io/api/docs-mcp`
- 🤝 **A2A agent** (16 skills) — `https://watchfor.io/api/a2a`
- 🧪 **No-auth sandbox** — `https://watchfor.io/api/v1/sandbox`
- 🩺 **Live diagnostics** (18 on-demand checks) — `https://watchfor.io/api/v1/diagnostics` · DNS, propagation, TLS grade, HTTP headers, ping, traceroute, ports, e-mail policy and more, run from the probe fleet. A model can reason about a site; it has no machine in 20 locations.
- 🧭 **WebMCP (in-page tools)** — nine browser-side tools on `document.modelContext`, so an agent-capable browser can use watchfor.io with no account · [audit](https://webmcp.ora.ai/watchfor.io)

## SDKs

| | |
| --- | --- |
| TypeScript | [`npm install watchfor`](https://www.npmjs.com/package/watchfor) |
| Python | [`pip install watchfor`](https://pypi.org/project/watchfor/) |
| Ruby | [`gem install watchfor`](https://rubygems.org/gems/watchfor) |

## Free tools — no signup

30+ free network & web tools at [watchfor.io/free-tools](https://watchfor.io/free-tools), including:

[Uptime calculator](https://watchfor.io/uptime-calculator) · [DNS checker](https://watchfor.io/dns-checker) · [DNS propagation](https://watchfor.io/dns-propagation-checker) · [HTTP header checker](https://watchfor.io/http-header-checker) · [Core Web Vitals checker](https://watchfor.io/core-web-vitals-checker) · [MCP server checker](https://watchfor.io/mcp-server-checker) · [Email header analyzer](https://watchfor.io/email-header-analyzer) · [DMARC](https://watchfor.io/dmarc-record-checker) / [DKIM](https://watchfor.io/dkim-record-checker) checkers · [Subnet calculator](https://watchfor.io/subnet-calculator) ([IPv6](https://watchfor.io/ipv6-subnet-calculator)) · [What's my IP](https://watchfor.io/whats-my-ip) · [Cron expression tester](https://watchfor.io/cron-expression-tester) · [Error budget calculator](https://watchfor.io/error-budget-calculator) · [JSON formatter](https://watchfor.io/json-formatter)

## Open source

- [`agent-toolkit`](https://github.com/watchfor-io/agent-toolkit) — AGENTS.md, agent skills, plugin manifest and MCP config

Agent quickstart: [watchfor.io/agents.md](https://watchfor.io/agents.md) · Docs: [watchfor.io/docs](https://watchfor.io/docs) · Engineering blog: [watchfor.io/blog](https://watchfor.io/blog) · Changelog: [watchfor.io/changelog](https://watchfor.io/changelog)
