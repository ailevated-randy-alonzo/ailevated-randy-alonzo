<div align="center">

<a href="https://portfolio.randyalonzo101.workers.dev"><img src="./assets/profile-cover.svg" width="100%" alt="Randy M. Alonzo — full-stack software engineering, backend systems, and cloud"/></a>

<br>

<strong>IT Support Specialist at Atos &nbsp;·&nbsp; Full-Stack Developer &nbsp;·&nbsp; Founder, AILEVATED</strong>

<p>From diagnosing user-facing incidents to designing APIs, I enjoy understanding <em>why systems behave the way they do</em>—and making them work better.</p>

<p>
<a href="https://portfolio.randyalonzo101.workers.dev"><img alt="Personal portfolio" src="https://img.shields.io/badge/PORTFOLIO-175B7D?style=for-the-badge&logo=cloudflare&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/randy-m-alonzo/"><img alt="LinkedIn" src="https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:randyalonzo101@gmail.com"><img alt="Email" src="https://img.shields.io/badge/CONTACT-233348?style=for-the-badge&logo=gmail&logoColor=white"/></a>
</p>

<sub>Manila, Philippines &nbsp; / &nbsp; Interested in software engineering, backend, and cloud roles</sub>

</div>

---

## Hello, I'm Randy.

I work in technical support and build full-stack applications. The overlap has shaped how I approach software: understand the user's problem, trace it through the system, decide where trust belongs, and explain failures clearly.

I'm developing toward a career in software engineering—particularly **backend services, cloud infrastructure, and products that need to be dependable in everyday use**.

Rather than listing every tool I've touched, I want the work to speak for itself.

### Pick a path through my work

| If you're looking for… | Start here |
|:--|:--|
| **Product thinking and end-to-end delivery** | [Hyrvanta](#01--hyrvanta--career-intelligence) and [JobPilot](#04--jobpilot--ai-career-workspace) |
| **Backend/API fundamentals** | [Storefront Admin](#03--storefront-admin--inventory-operations) |
| **Integration reliability and failure handling** | [Nearby Nook](#02--nearby-nook--local-discovery) |
| **A deeper technical review** | [Engineering notes with code references](./docs/engineering-notes.md) |

---

## Selected work

### 01 · Hyrvanta — career intelligence

**React 19 · TypeScript · Cloudflare Workers · D1 · R2**

<a href="https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/main/public/og.png" width="100%" alt="Hyrvanta software project preview from its repository"/></a>

**The question:** How can a career platform recommend next steps without inventing job evidence or exposing someone’s résumé?

I built a workspace for job discovery, application tracking and career evidence. The important work happens behind the interface:

- **Ownership:** authenticated API routes use the user's identity to scope records.
- **Data:** D1 stores application and Career Vault metadata; private R2 stores résumé files.
- **Integrations:** Greenhouse and Lever adapters normalize job records and apply source, URL and freshness rules.
- **Verification:** domain and route tests, React UI checks, typechecking and rendered-output tests are defined in the repository.

**Architecture — the boundaries that matter**

<a href="https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/current-architecture.md"><img src="./assets/hyrvanta-architecture.svg" width="100%" alt="Hyrvanta system architecture with React client, authenticated API, Cloudflare D1/R2, and employer synchronization adapters"/></a>

The user interface is not the authority for access control. The API owns authorization, and files are kept separate from the public application assets.

**Inspect:** [Repository](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence) · [API implementation](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/app/api/jobs/route.ts) · [Job adapters](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/lib/job-sources.ts) · [Security notes](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/security.md) · [Tests](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/tree/main/tests)

<sub>Release note: portfolio-ready working release. Production identity, real employer-source setup, extension pairing and monitoring still require additional configuration or development. Preview vacancies are labeled rather than presented as live.</sub>

---

### 02 · Nearby Nook — local discovery

**React · Node.js · Leaflet · OpenStreetMap**

<a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/nearby-nook-local-discovery/main/docs/screenshots/nearby-nook-map-results.png" width="100%" alt="Nearby Nook map results and location discovery interface"/></a>

**The question:** What should a location app do when its data provider is slow, incomplete or unavailable?

The answer is not to invent a nearby place. I used a same-origin Node API to isolate OpenStreetMap providers from the React interface.

<a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/docs/architecture.md"><img src="./assets/nearby-architecture.svg" width="100%" alt="Nearby Nook architecture with React Leaflet, same-origin Node API, cache and Nominatim and Overpass provider integrations"/></a>

A testable gateway handles **input validation, TTL caching, request coalescing, upstream timeouts and Overpass fallback**. Development fixtures are clearly separated from live production data.

**Inspect:** [Repository](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery) · [Gateway code](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/server/osmGateway.js) · [Caching](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/server/cache.js) · [Gateway tests](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/server/osmGateway.test.js)

---

<table>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard/main/assets/screenshots/dashboard-dark.png" width="100%" alt="Storefront Admin inventory dashboard"/></a>
<h3>03 · Storefront Admin — inventory operations</h3>
<p><b>Node.js · Express · MySQL</b></p>
<p>Inventory CRUD with searchable products, stock views and protected administrator operations. The API handles validation, bcrypt password checks and signed, expiring sessions.</p>
<p><a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard"><b>Repository</b></a> · <a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard/blob/main/server.js">Backend source</a> · <a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard#api-routes">API routes</a></p>
</td>
<td width="50%" valign="top">
<a href="https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/jobpilot-career-copilot/main/docs/screenshots/jobpilot-dashboard.png" width="100%" alt="JobPilot career copilot dashboard"/></a>
<h3>04 · JobPilot — AI career workspace</h3>
<p><b>React · TypeScript · Cloudflare · OpenAI API</b></p>
<p>Application and private résumé management with evidence-backed role comparisons. AI requests stay server-side, with structured outputs and resource ownership checks.</p>
<p><a href="https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot"><b>Repository</b></a> · <a href="https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot/tree/main/app/api">API routes</a> · <a href="https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot/tree/main/docs/screenshots">Product tour</a></p>
</td>
</tr>
</table>

<sub>Project screenshots are sourced from their repositories. JobPilot's hosted workspace requires authorized access; a local demonstration path is described in its README.</sub>

**More projects:** [Personal portfolio](https://github.com/ailevated-randy-alonzo/randy-alonzo-portfolio) · [AILEVATED AI platform](https://github.com/ailevated-randy-alonzo/ailevated-ai-platform)

---

## Engineering decisions worth inspecting

<a href="./docs/engineering-notes.md"><img src="./assets/engineering-evidence.svg" width="100%" alt="Engineering evidence — security, resilience, quality, and API design"/></a>

There are four questions I try to answer before calling a feature finished:

**01 / Who is allowed to access the data?**  
In Hyrvanta, authorization belongs on the API—not in React state. [Inspect the authenticated job route](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/app/api/jobs/route.ts) and [security model](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/security.md).

**02 / What happens when a dependency fails?**  
Nearby Nook uses server-side timeouts, caching, request coalescing, and fallback between public data providers. [Read the gateway](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/server/osmGateway.js) and [cache implementation](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/server/cache.js).

**03 / How do I know it works?**  
Tests aren't a badge: they should exercise meaningful behavior. [Hyrvanta test scripts](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/package.json) cover domain, UI, and rendered output; [Nearby Nook gateway tests](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/server/osmGateway.test.js) cover service responses.

**04 / Can another engineer understand the contract?**  
Storefront Admin documents CRUD routes, session handling, and input validation. [Read the actual Express implementation](https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard/blob/main/server.js).

**[Open my engineering review notes →](./docs/engineering-notes.md)** — architecture, evidence, tradeoffs, and limitations behind the project showcase.

---

## Engineering toolkit

<img src="./assets/engineering-focus.svg" width="100%" alt="Color-coded engineering capabilities for applications, backend systems, cloud and IT operations"/>

My most-used project technologies are **TypeScript, JavaScript, React, Node.js, Express, MySQL, Cloudflare Workers, D1, and R2**. I also work with Git/GitHub, Vitest, ESLint, input validation, authentication, and access-control patterns.

In IT operations, my day-to-day foundation includes **Windows, Microsoft 365, networking fundamentals, issue triage, and documentation**.

The four areas above aren't equal claims of expertise. They describe tools and responsibilities demonstrated in source code or professional experience. When a reviewer wants more detail, the linked repositories show the implementation.

---

## Background & professional journey

<img src="./assets/professional-journey.svg" width="100%" alt="Professional experience timeline: Atos IT Support, B.S. Information Technology at TUP Manila, and AILEVATED"/>

**Atos — IT Support Specialist**  
First-line incident triage, hardware/software troubleshooting, escalation, and documentation. It has taught me to value reproducible problems, user impact, and clear handovers.

**Technological University of the Philippines–Manila — B.S. Information Technology**  
Academic work in software, databases, networking, and information systems.

**AILEVATED — Founder**  
I build technical learning resources, software projects, and practical AI workflows for an audience of learners and professionals.

I'm pursuing **software engineering opportunities** with teams that care about correctness, maintainability, helpful feedback, and the people who depend on the software.

---

## Let's work together

<a href="mailto:randyalonzo101@gmail.com"><img src="./assets/connect-editorial.svg" width="100%" alt="Let's build something useful — engineering opportunities and collaborations with Randy M. Alonzo"/></a>

<div align="center">

<a href="mailto:randyalonzo101@gmail.com"><img src="https://img.shields.io/badge/EMAIL_ME-167E99?style=for-the-badge&logo=gmail&logoColor=white" alt="Email me"></a>
<a href="https://www.linkedin.com/in/randy-m-alonzo/"><img src="https://img.shields.io/badge/CONNECT_ON_LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
<a href="https://portfolio.randyalonzo101.workers.dev"><img src="https://img.shields.io/badge/VIEW_PORTFOLIO-1B526F?style=for-the-badge&logo=cloudflare&logoColor=white" alt="Portfolio"></a>

**Professional:** [GitHub](https://github.com/ailevated-randy-alonzo) · [Email](mailto:randyalonzo101@gmail.com) · [LinkedIn](https://www.linkedin.com/in/randy-m-alonzo/)

**Learning & community:** [AWS Builder — achievements and badges](https://builder.aws.com/community/@ranbyruz?tab=badges) · [AILEVATED](https://ailevated.tech) · [YouTube](https://www.youtube.com/@ailevated)

**Freelance & collaboration:** [Fiverr services](https://www.fiverr.com/sellers/ailevated/) · [Upwork profile](https://www.upwork.com/freelancers/~01e817b1de0c60f604?viewMode=1&mp_source=share)

<sub>Built with curiosity, systems thinking, and a commitment to improving real software.</sub>

</div>
