<div align="center">

<a href="https://portfolio.randyalonzo101.workers.dev">
<img src="./assets/profile-cover.svg" alt="Randy M. Alonzo, software engineering portfolio focused on full-stack development, backend APIs and cloud systems" width="100%">
</a>

### Hi, I'm Randy. I troubleshoot real systems—and build software to make them better.

I'm an IT support specialist and a developer with a particular interest in **backend engineering, cloud infrastructure, and trustworthy products**.

<p>
<a href="https://portfolio.randyalonzo101.workers.dev"><img src="https://img.shields.io/badge/PORTFOLIO-146C99?style=for-the-badge&logo=cloudflare&logoColor=white" alt="Portfolio"></a>
<a href="https://www.linkedin.com/in/randy-m-alonzo/"><img src="https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
<a href="mailto:randyalonzo101@gmail.com"><img src="https://img.shields.io/badge/EMAIL-1E344C?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

<sub>Manila, Philippines &nbsp;·&nbsp; IT Support Specialist at Atos &nbsp;·&nbsp; Founder, AILEVATED</sub>

[Featured work](#selected-engineering-work) &nbsp;·&nbsp; [Architecture](#architecture-behind-the-project) &nbsp;·&nbsp; [Technical strengths](#how-i-approach-engineering) &nbsp;·&nbsp; [Contact](#connect)

</div>

---

## What I bring to engineering

Working in technical support has made me attentive to something that is easy to overlook when building applications: **what happens when the expected path fails?**

That perspective shapes my projects. I focus on clear user experiences, predictable APIs, careful handling of private data, and implementations that another developer can inspect and run.

I am building toward a software engineering career in teams working on **backend systems, cloud services, developer tools, and product reliability**.

| I build | I pay attention to | I bring from support |
|:--|:--|:--|
| Web apps and REST APIs | Authorization, validation, tests, failure states | Triage, reproducibility, documentation |

## Selected engineering work

### 01 — Hyrvanta / evidence-first career intelligence

**The challenge:** How do you help someone evaluate opportunities and tailor a résumé *without inventing evidence or exposing personal records?*

<a href="https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/main/public/og.png" width="100%" alt="Hyrvanta project preview from the application repository"></a>

**The product:** An application and career-evidence workspace, with employer-board adapters, saved opportunities, private résumé versions, and user-controlled application tracking.

**The engineering:**

- **API security:** Authenticated, owner-scoped routes protect application records and résumé access.
- **Data boundaries:** D1 handles structured records; private R2 handles document files.
- **External data:** Greenhouse and Lever adapters normalize incoming jobs and apply verification, freshness, deduplication and URL-safety rules.
- **Verification:** The repository defines domain and route tests, React interaction tests, TypeScript checking, linting and rendered-page checks.

<sub>React 19 · TypeScript · Cloudflare Workers · D1 · R2 · Drizzle ORM · Vitest</sub>

**Explore the implementation:** [Code](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence) · [Architecture](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/current-architecture.md) · [Security model](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/security.md) · [Test suite](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/tree/main/tests)

#### Architecture behind the project

<a href="https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/current-architecture.md"><img src="./assets/hyrvanta-architecture.svg" width="100%" alt="Architecture of Hyrvanta from browser to authenticated API and D1/R2, with separate employer-feed synchronization"></a>

**In plain English:** the browser talks to authenticated server routes. The server checks record ownership before accessing structured data or private files. Job-source adapters use a separate ingestion path rather than exposing providers directly to the browser.

<sub>Scope: a portfolio-ready working release. Production identity, employer-source configuration, extension pairing, and monitoring still need additional setup or implementation. Sample listings are labeled as previews.</sub>

---

### 02 — Nearby Nook / local discovery without invented data

<table>
<tr>
<td width="45%" valign="top">
<a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/nearby-nook-local-discovery/main/docs/screenshots/nearby-nook-map-results.png" width="100%" alt="Actual Nearby Nook map-search application screenshot"></a>
</td>
<td valign="top">
<b>The challenge:</b> Public place data can be incomplete or temporarily unavailable.<br><br>
<b>The build:</b> A React/Leaflet map with a same-origin Node API.<br><br>
<b>The decision:</b> Put caching, validation, rate limiting and Overpass provider failover on the server. Don't silently replace unavailable live results with fictional places.<br><br>
<a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery"><b>Repository</b></a> · <a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/docs/architecture.md">Architecture</a> · <a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/server/osmGateway.test.js">Gateway tests</a>
</td>
</tr>
</table>

<sub>React · Node.js · Leaflet · OpenStreetMap · Vitest</sub>

### 03 — Storefront Admin / full-stack inventory operations

<table>
<tr>
<td width="45%" valign="top">
<a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard/main/assets/screenshots/dashboard-dark.png" width="100%" alt="Actual Storefront Admin inventory dashboard screenshot"></a>
</td>
<td valign="top">
<b>The challenge:</b> Product updates need consistent validation and protected write operations.<br><br>
<b>The build:</b> An inventory dashboard with search, stock views and product CRUD.<br><br>
<b>The decision:</b> Use an Express API backed by MySQL, with bcrypt verification, signed sessions and server-side input checks.<br><br>
<a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard"><b>Repository</b></a> · <a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard/blob/main/server.js">Backend source</a> · <a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard#api-routes">API contract</a>
</td>
</tr>
</table>

<sub>JavaScript · Node.js · Express · MySQL</sub>

### 04 — JobPilot / grounded AI career workflows

<table>
<tr>
<td width="45%" valign="top">
<a href="https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/jobpilot-career-copilot/main/docs/screenshots/jobpilot-dashboard.png" width="100%" alt="Actual JobPilot application dashboard screenshot"></a>
</td>
<td valign="top">
<b>The challenge:</b> AI-generated job advice can sound convincing without reflecting a person's real experience.<br><br>
<b>The build:</b> An application tracker, private résumé library and evidence-backed interview preparation.<br><br>
<b>The decision:</b> Keep API keys and AI requests server-side, protect résumé files with ownership checks and request structured outputs.<br><br>
<a href="https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot"><b>Repository</b></a> · <a href="https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot/tree/main/docs/screenshots">Product walkthrough</a>
</td>
</tr>
</table>

<sub>React · TypeScript · Cloudflare D1/R2 · OpenAI Responses API</sub>

<sub>JobPilot's hosted workspace requires authorized access. The repository provides local demonstration instructions.</sub>

<details>
<summary><b>Two more projects — portfolio website &amp; AILEVATED</b></summary>

- **[Personal portfolio](https://github.com/ailevated-randy-alonzo/randy-alonzo-portfolio)** — professional experience, technical projects and practical learning. [See the live website](https://portfolio.randyalonzo101.workers.dev).
- **[AILEVATED AI platform](https://github.com/ailevated-randy-alonzo/ailevated-ai-platform)** — a responsive AI-tools and learning-resources interface.

</details>

---

## How I approach engineering

| Principle | What you can inspect |
|:--|:--|
| **Secure the boundary** | [Hyrvanta's owner-scoped reads and private file access](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/security.md) |
| **Make failures explicit** | [Nearby Nook's provider timeouts, caching and error handling](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/docs/architecture.md) |
| **Keep API behavior understandable** | [Storefront Admin's routes and validation](https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard/blob/main/server.js) |
| **Test what matters** | [Hyrvanta's verification scripts](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/package.json) · [Nearby Nook's Vitest suite](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/package.json) |

<details>
<summary><b>Engineering tradeoffs and next improvements</b></summary>

- **Hyrvanta:** complete production identity/integration configuration and expand monitoring, rate limiting and browser-extension pairing.
- **Nearby Nook:** replace process-local caching and throttling with shared services before any multi-instance deployment.
- **Storefront Admin:** extend automated API and integration test coverage; remove demo credentials before public use.
- **JobPilot:** expand end-to-end and accessibility checks; offer a public demonstration with synthetic data.

These are engineering follow-ups, not claims of already delivered production capabilities.

</details>

## Technical toolkit

<table>
<tr>
<td width="50%" valign="top">
<b>Software engineering</b><br>
TypeScript · JavaScript · React · Node.js · Express · HTML/CSS · REST APIs
</td>
<td width="50%" valign="top">
<b>Cloud, data &amp; quality</b><br>
Cloudflare Workers · D1 · R2 · Drizzle ORM · MySQL · Git · Vitest · ESLint
</td>
</tr>
</table>

**IT operations:** Windows, Microsoft 365, networking fundamentals, issue triage, technical documentation and escalation.

The technologies above reflect project work and professional exposure; depth varies. Source code and architectural explanations are linked so you can evaluate the work yourself.

## Beyond the code

**Atos — IT Support Specialist**  
First-line technical support, troubleshooting, documentation and escalation.

**Technological University of the Philippines–Manila — B.S. Information Technology**  
Academic foundation in information technology, software and systems.

**AILEVATED — Founder**  
Technology education, practical AI workflows, original learning content and digital products.

---

## Connect

<div align="center">

**Interested in engineering work, collaboration, or a project discussion?**

[**View my portfolio**](https://portfolio.randyalonzo101.workers.dev) &nbsp;·&nbsp; [**Connect on LinkedIn**](https://www.linkedin.com/in/randy-m-alonzo/) &nbsp;·&nbsp; [**Email me**](mailto:randyalonzo101@gmail.com)

</div>

| Professional | Creator &amp; freelance work |
|:--|:--|
| [✉️ randyalonzo101@gmail.com](mailto:randyalonzo101@gmail.com) | [🎨 Fiverr — AILEVATED](https://www.fiverr.com/sellers/ailevated/) |
| [🌐 Portfolio](https://portfolio.randyalonzo101.workers.dev) | [💼 Upwork profile](https://www.upwork.com/freelancers/~01e817b1de0c60f604?viewMode=1&mp_source=share) |
| [💼 LinkedIn](https://www.linkedin.com/in/randy-m-alonzo/) | [☁️ AWS Builder badges](https://builder.aws.com/community/@ranbyruz?tab=badges) |
| [🐙 GitHub repositories](https://github.com/ailevated-randy-alonzo) | [🚀 AILEVATED](https://ailevated.tech) · [▶️ YouTube](https://www.youtube.com/@ailevated) |

<div align="center"><sub>Real projects. Clear decisions. An engineering practice that keeps improving.</sub></div>
