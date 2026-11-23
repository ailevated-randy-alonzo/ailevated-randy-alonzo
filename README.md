# Randy M. Alonzo

**Full-stack developer · IT Support Specialist at Atos**  
Manila, Philippines · B.S. Information Technology, TUP Manila (in progress)

I work in frontline IT support and build web applications outside that role. Support taught me to investigate problems from the user's side; writing software gives me a way to address them in the product itself.

I'm moving toward software engineering, particularly backend development and cloud-based applications. Below is work you can inspect—not a list of technologies I hope to learn.

[**Portfolio**](https://portfolio.randyalonzo101.workers.dev) · [LinkedIn](https://www.linkedin.com/in/randy-m-alonzo/) · [Email](mailto:randyalonzo101@gmail.com)

---

## Selected work

### 01 / [Hyrvanta — Career Intelligence](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence)

**React · TypeScript · Cloudflare Workers · D1 · R2 · Drizzle**

A career workspace built around a specific constraint: job opportunities and résumé claims should be traceable to evidence rather than silently inferred.

- **Data boundary:** authenticated, owner-scoped APIs; D1 records for career data; private R2 storage for résumé files.
- **External sources:** Greenhouse and Lever adapters with source validation, deduplication, freshness rules, timeouts, and retries. Jooble support is optional.
- **Checks:** the repository defines domain/route tests, React interaction tests, TypeScript checks, linting, a production build, and rendered-HTML checks.

**Explore:** [Architecture](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/current-architecture.md) · [Security model](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/security.md) · [Test suite](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/tree/main/tests) · [Source code](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence)

<sub>Project scope: a working portfolio release. Production identity, employer-source configuration, extension pairing, and some integrations still require setup or further implementation. Preview opportunities are labeled.</sub>

### 02 / [Nearby Nook — Local Discovery](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery)

**React · Node.js · Leaflet · OpenStreetMap · Vitest**

A map-based neighborhood explorer with a deliberately small server boundary between the browser and public location providers.

- **API design:** a same-origin Node API validates requests, manages caching and coalescing, applies per-client limits, and handles provider timeouts/failover.
- **Data honesty:** missing place details stay missing; development-only fixture data is not silently served as real production listings.
- **Checks:** `npm run check` runs Vitest and produces a Vite build.

**Explore:** [Architecture and tradeoffs](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/docs/architecture.md) · [Application tests](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/tree/main/tests) · [Source code](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery)

### 03 / [Storefront Admin — Inventory Dashboard](https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard)

**Node.js · Express · MySQL · JavaScript**

An inventory management app built around ordinary but important backend workflows: sign-in, product records, validation, and stock visibility.

- **Backend:** REST endpoints for product CRUD, server-side input validation, bcrypt password verification, and signed, expiring sessions.
- **Frontend:** responsive inventory views, product search/filtering, confirmation states, and stock summaries.

**Explore:** [API and setup documentation](https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard#api-routes) · [Server implementation](https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard/blob/main/server.js) · [Source code](https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard)

### 04 / [JobPilot — AI Career Copilot](https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot)

**React · TypeScript · Cloudflare D1/R2 · OpenAI Responses API**

An authenticated application tracker with private résumé files and role comparisons that identify supporting evidence and skill gaps.

- AI calls happen server-side with structured outputs; résumé and application records are subject to ownership checks.
- The hosted workspace is private. The repository documents its local demonstration path and current boundaries.

**Explore:** [Project walkthrough and architecture](https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot) · [Application screenshots](https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot/tree/main/docs/screenshots)

---

### From the actual applications

<table>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery">
<img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/nearby-nook-local-discovery/main/docs/screenshots/nearby-nook-map-results.png" width="100%" alt="Nearby Nook application screenshot showing an interactive map and search results" />
</a>
<br/><sub><b>Nearby Nook</b> — map and place results. <a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/tree/main/docs/screenshots">More captures</a></sub>
</td>
<td width="50%" valign="top">
<a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard">
<img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard/main/assets/screenshots/dashboard-dark.png" width="100%" alt="Storefront Admin application screenshot showing the inventory dashboard" />
</a>
<br/><sub><b>Storefront Admin</b> — inventory dashboard. <a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard/tree/main/assets/screenshots">More captures</a></sub>
</td>
</tr>
</table>

These are screenshots stored in the linked project repositories, not illustrations created for this profile.

**Additional projects:** [Personal portfolio](https://github.com/ailevated-randy-alonzo/randy-alonzo-portfolio) · [AILEVATED learning platform](https://github.com/ailevated-randy-alonzo/ailevated-ai-platform)

## Engineering details I pay attention to

| Concern | Example to review |
| --- | --- |
| **Ownership and privacy** | [Hyrvanta's server-side access boundaries](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/security.md) |
| **Unreliable dependencies** | [Nearby Nook's OpenStreetMap gateway, caching, and failover](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/docs/architecture.md) |
| **Backend fundamentals** | [Storefront Admin's validation, authentication, and product APIs](https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard) |
| **Verification** | [Hyrvanta's checks](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/package.json) and [Nearby Nook's test/build workflow](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/package.json) |

I'm comfortable discussing what these projects **do not** yet cover. A working portfolio release is not the same thing as a production system with observed traffic, operational SLOs, and mature deployment controls.

## Background

- **Atos — IT Support Specialist:** first-line support, troubleshooting, issue triage, escalation, and documentation.
- **Technological University of the Philippines–Manila:** B.S. in Information Technology, ongoing.
- **AILEVATED:** I publish practical technical learning material and build tools around AI, development, and IT.

**Languages and technologies used in the projects above:** TypeScript, JavaScript, React, Node.js, Express, SQL/MySQL, Cloudflare Workers/D1/R2, Git, Vitest. My IT support work also involves Windows, Microsoft 365, and networking fundamentals.

## Contact

For engineering opportunities or project discussions: **[randyalonzo101@gmail.com](mailto:randyalonzo101@gmail.com)**

[Portfolio](https://portfolio.randyalonzo101.workers.dev) · [LinkedIn](https://www.linkedin.com/in/randy-m-alonzo/) · [GitHub](https://github.com/ailevated-randy-alonzo)

**Elsewhere:** [AWS Builder — badges](https://builder.aws.com/community/@ranbyruz?tab=badges) · [Fiverr](https://www.fiverr.com/sellers/ailevated/) · [Upwork](https://www.upwork.com/freelancers/~01e817b1de0c60f604?viewMode=1&mp_source=share) · [AILEVATED](https://ailevated.tech) · [YouTube](https://www.youtube.com/@ailevated)
