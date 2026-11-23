<div align="center">

<a href="https://portfolio.randyalonzo101.workers.dev"><img src="./assets/profile-cover.svg" alt="Randy M. Alonzo — software engineering portfolio focused on full-stack products, backend APIs, and cloud systems" width="100%"/></a>

### Building software with an operator's perspective.

I'm **Randy M. Alonzo** — a full-stack developer and IT support specialist. I build software, investigate failure paths, and care about making complex systems understandable to the people who use them.

<p>
<a href="https://portfolio.randyalonzo101.workers.dev"><img alt="Explore portfolio" src="https://img.shields.io/badge/EXPLORE_PORTFOLIO-1378A9?style=for-the-badge&logo=cloudflare&logoColor=white" /></a>
<a href="https://www.linkedin.com/in/randy-m-alonzo/"><img alt="Connect on LinkedIn" src="https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="mailto:randyalonzo101@gmail.com"><img alt="Email Randy" src="https://img.shields.io/badge/EMAIL-22364F?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>

<sub>Manila, Philippines &nbsp; · &nbsp; IT Support Specialist, Atos &nbsp; · &nbsp; Founder, AILEVATED</sub>

</div>

---

## The work, not just the stack.

My professional background is in **technical support and incident troubleshooting**. My development work extends that mindset into product design, APIs, authorization, data modeling, and testing.

I'm interested in software engineering opportunities where strong fundamentals matter: **backend systems, cloud platforms, developer tooling, reliability, and products used by real people**.

<table>
<tr>
<td width="33%" valign="top"><b>PRODUCT ENGINEERING</b><br/><sub>React · TypeScript · accessible interfaces</sub></td>
<td width="34%" valign="top"><b>BACKEND &amp; DATA</b><br/><sub>Node.js · REST APIs · SQL · ownership boundaries</sub></td>
<td width="33%" valign="top"><b>SYSTEMS THINKING</b><br/><sub>Cloudflare · tests · debugging · operational tradeoffs</sub></td>
</tr>
</table>

## 01 / Featured engineering work

### [Hyrvanta — career intelligence with traceable evidence](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence)

<sub>React 19 · TypeScript · Cloudflare Workers · D1 · R2 · Drizzle ORM</sub>

<a href="https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/main/public/og.png" alt="Hyrvanta project product preview" width="100%" /></a>

Hyrvanta explores a challenge I care about: **how can job-search software help people make better decisions without inventing evidence or exposing private career data?**

The project combines job-source normalization, application tracking, résumé versioning, and a structured Career Vault. The implementation deliberately separates *preview data* from verified sources and requires user control over material actions.

| Engineering decision | Why I made it |
|:--|:--|
| **Authenticated, owner-scoped API routes** | Authorization is enforced on the server, not assumed from the user interface. |
| **Cloudflare D1 + private R2** | Structured application metadata and résumé files have different storage and access requirements. |
| **Employer-source adapters** | Greenhouse/Lever data passes through URL-safety, normalization, deduplication, and freshness checks. |
| **Evidence-first outputs** | Material résumé claims remain linked to user-supplied records rather than silently inferred. |

**Read the engineering evidence:** [Source code](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence) · [Architecture notes](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/current-architecture.md) · [Security boundaries](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/security.md) · [Tests](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/tree/main/tests)

#### System architecture / Hyrvanta

<a href="https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/current-architecture.md"><img src="./assets/hyrvanta-architecture.svg" alt="Hyrvanta architecture: React client to authenticated Worker API to Cloudflare D1 and private R2; Greenhouse and Lever data enters through server-side normalization" width="100%" /></a>

<sub>Architecture distilled from the repository's implementation notes. This is a working portfolio release; production identity, employer configuration, pairing, monitoring, and other integrations require additional setup. I do not present preview listings as live vacancies.</sub>

---

## 02 / More systems I've built

<table>
<tr>
<td width="43%" valign="top">
<a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/nearby-nook-local-discovery/main/docs/screenshots/nearby-nook-map-results.png" width="100%" alt="Nearby Nook application screenshot showing real UI with map and place results" /></a>
</td>
<td valign="top">
<h3><a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery">Nearby Nook</a></h3>
<b>Location discovery · React / Node.js / OpenStreetMap</b>
<p>A guest-first map application that separates browser interaction from third-party location services.</p>
<p><b>Engineering focus:</b> Same-origin Node API, validated requests, short-lived caching, per-client limits, and Overpass provider failover.</p>
<a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/docs/architecture.md">Architecture &amp; tradeoffs</a> · <a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/server/osmGateway.test.js">API tests</a>
</td>
</tr>
<tr>
<td width="43%" valign="top">
<a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard/main/assets/screenshots/dashboard-dark.png" width="100%" alt="Actual Storefront Admin dark-mode inventory dashboard" /></a>
</td>
<td valign="top">
<h3><a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard">Storefront Admin</a></h3>
<b>Inventory CRUD · Node.js / Express / MySQL</b>
<p>An authenticated inventory dashboard connecting product workflows to a relational database.</p>
<p><b>Engineering focus:</b> Product CRUD, validated API routes, signed sessions, password verification, and inventory summaries.</p>
<a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard/blob/main/server.js">Backend implementation</a> · <a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard#api-routes">API documentation</a>
</td>
</tr>
<tr>
<td width="43%" valign="top">
<a href="https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/jobpilot-career-copilot/main/docs/screenshots/jobpilot-dashboard.png" width="100%" alt="Actual JobPilot application dashboard" /></a>
</td>
<td valign="top">
<h3><a href="https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot">JobPilot</a></h3>
<b>Evidence-backed AI workflow · React / TypeScript / Cloudflare</b>
<p>A private application and résumé workspace that turns job descriptions into grounded interview preparation.</p>
<p><b>Engineering focus:</b> Authenticated records, R2 file access controls, server-side OpenAI requests, and structured outputs.</p>
<a href="https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot">Code &amp; documentation</a> · <a href="https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot/tree/main/docs/screenshots">Product walkthrough</a>
</td>
</tr>
</table>

<sub>These are actual project assets from the linked repositories. JobPilot's hosted workspace currently requires authorized access; its README documents the local demonstration environment.</sub>

<details>
<summary><b>Also in my portfolio · Personal website &amp; AILEVATED platform</b></summary>

- [Personal portfolio](https://github.com/ailevated-randy-alonzo/randy-alonzo-portfolio) — technical support experience, development work, and learning in one place. [View live website](https://portfolio.randyalonzo101.workers.dev).
- [AILEVATED AI platform](https://github.com/ailevated-randy-alonzo/ailevated-ai-platform) — a responsive AI tools, prompts, and learning-resources interface.

</details>

---

## 03 / How I think about engineering

A polished interface matters, but the implementation behind it matters more. These are the areas I intentionally practice and document:

| Area | Evidence in my work |
|:--|:--|
| **Security boundaries** | [Owner-scoped data, private files, and server-side authorization](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/security.md) |
| **Resilience** | [Cache/coalescing, provider failover, timeouts, and explicit fallback behavior](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/docs/architecture.md) |
| **Testability** | [Hyrvanta's domain, route, UI, and rendered-HTML checks](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/package.json) · [Nearby Nook's test/build scripts](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/package.json) |
| **Backend fundamentals** | [REST contracts, sessions, validation, and MySQL product persistence](https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard) |
| **Responsible AI integration** | [Evidence-backed comparisons, private uploads, and server-side generation](https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot) |

<details>
<summary><b>What I'd improve next · Engineering tradeoffs, not fictional metrics</b></summary>

- **Hyrvanta:** finalize production identity and integration configuration; add rate limiting, security hardening, monitoring, and a signed browser-extension pairing flow.
- **Nearby Nook:** move process-local throttling/caching to shared infrastructure for any multi-instance deployment; finish authenticated sync only after an identity provider is chosen.
- **Storefront Admin:** expand automated API/integration tests and harden the documented demo account before public deployment.
- **JobPilot:** strengthen end-to-end and accessibility testing; its hosted experience remains access restricted.

I describe these as future improvements—not as capabilities already delivered.

</details>

## 04 / Technical toolkit

<p>
<img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
<img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F4CC43?style=flat-square&logo=javascript&logoColor=20252D"/>
<img alt="React" src="https://img.shields.io/badge/React-149ECA?style=flat-square&logo=react&logoColor=white"/>
<img alt="Node.js" src="https://img.shields.io/badge/Node.js-3C873A?style=flat-square&logo=nodedotjs&logoColor=white"/>
<img alt="Express" src="https://img.shields.io/badge/Express-303F54?style=flat-square&logo=express&logoColor=white"/>
<img alt="MySQL" src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
<img alt="Cloudflare" src="https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white"/>
<img alt="Vitest" src="https://img.shields.io/badge/Vitest-729B1E?style=flat-square&logo=vitest&logoColor=white"/>
</p>

**Application:** React, TypeScript, JavaScript, HTML/CSS, Node.js, Express  
**Cloud & data:** Cloudflare Workers, D1, R2, Drizzle ORM, MySQL, SQL, REST APIs  
**Development practices:** Git/GitHub, Vitest, TypeScript checks, ESLint, input validation, auth/access control  
**IT & systems:** Windows, Microsoft 365, networking, incident triage, documentation

Technology depth varies by project. I prefer showing code and documented decisions over claiming expertise in every tool.

## 05 / Professional background

**IT Support Specialist · Atos** — First-line support, technical troubleshooting, documentation, and escalation.

**B.S. Information Technology · Technological University of the Philippines–Manila** — My academic foundation in software, infrastructure, and systems.

**Founder · AILEVATED** — Technology education, project-based learning, and practical AI resources.

My next chapter is in **software engineering**. I'm especially motivated by teams working on backend systems, cloud services, reliability, developer experience, and products where careful design improves the user experience.

---

## Contact & collaboration

<div align="center">

**Engineering opportunity, technical discussion, or a project worth building?**

<a href="mailto:randyalonzo101@gmail.com"><img alt="Email Randy" src="https://img.shields.io/badge/LET'S_TALK-1495B5?style=for-the-badge&logo=gmail&logoColor=white"/></a>

</div>

| Engineering & career | Community & client work |
|:--|:--|
| [Email — randyalonzo101@gmail.com](mailto:randyalonzo101@gmail.com) | [Fiverr — AILEVATED services](https://www.fiverr.com/sellers/ailevated/) |
| [Personal portfolio](https://portfolio.randyalonzo101.workers.dev) | [Upwork — freelancer profile](https://www.upwork.com/freelancers/~01e817b1de0c60f604?viewMode=1&mp_source=share) |
| [LinkedIn — Randy M. Alonzo](https://www.linkedin.com/in/randy-m-alonzo/) | [AWS Builder — learning badges](https://builder.aws.com/community/@ranbyruz?tab=badges) |
| [GitHub — source code](https://github.com/ailevated-randy-alonzo) | [AILEVATED](https://ailevated.tech) · [YouTube](https://www.youtube.com/@ailevated) |

<div align="center">
<sub>Built to be explored, questioned, and improved. © 2026 Randy M. Alonzo.</sub>
</div>
