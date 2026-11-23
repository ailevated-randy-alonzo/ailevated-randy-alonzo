<div align="center">

<a href="https://portfolio.randyalonzo101.workers.dev">
  <img src="./assets/profile-cover.svg" alt="Randy M. Alonzo — full-stack development, backend systems, cloud | Featured projects: Hyrvanta, Nearby Nook, Storefront Admin, and JobPilot" width="100%" />
</a>

### I build software with the same mindset I bring to solving real IT problems.

Developer and IT support specialist focused on **usable applications, dependable APIs, and thoughtful system design.**

<p>
  <a href="https://portfolio.randyalonzo101.workers.dev"><img alt="Portfolio" src="https://img.shields.io/badge/PORTFOLIO-1683AF?style=for-the-badge&logo=cloudflare&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/randy-m-alonzo/"><img alt="LinkedIn" src="https://img.shields.io/badge/LINKEDIN-19577C?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:randyalonzo101@gmail.com"><img alt="Email" src="https://img.shields.io/badge/EMAIL-1E344C?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>

<sub>Metro Manila, Philippines · IT Support Specialist at Atos · B.S. Information Technology, TUP Manila (in progress) · Founder of AILEVATED</sub>

</div>

---

## About me

I'm **Randy M. Alonzo**, a full-stack developer and IT support professional. My day-to-day work involves troubleshooting and helping people through technical issues. My development projects take that same problem-solving approach into interfaces, APIs, data handling, and cloud services.

I'm especially interested in **backend engineering and cloud-based systems**. The projects below show what I've implemented, how I organized it, and which parts are still in progress.

<table>
<tr>
<td width="33%" valign="top"><b>BUILD</b><br/><sub>Full-stack interfaces, REST APIs, SQL, cloud services</sub></td>
<td width="33%" valign="top"><b>VALIDATE</b><br/><sub>Ownership checks, testing, source verification, error handling</sub></td>
<td width="33%" valign="top"><b>SUPPORT</b><br/><sub>Windows, Microsoft 365, service desk operations, documentation</sub></td>
</tr>
</table>

## Selected engineering work

<sub>Four projects, four different technical problems. Each image below comes from the corresponding project's own repository.</sub>

<table>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/main/public/og.png" alt="Actual Hyrvanta product preview" width="100%" /></a>
<h3>01 — Hyrvanta</h3>
<p><b>Career intelligence &amp; private data</b></p>
<p>A career platform that separates verified opportunity data from previews and links résumé claims to supporting evidence.</p>
<p><sub><b>Engineering:</b> Owner-scoped API routes, D1 records, private R2 files, Greenhouse/Lever adapters, and tests.</sub></p>
<p><a href="https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence"><b>Source code</b></a> · <a href="https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/current-architecture.md">Architecture</a></p>
</td>
<td width="50%" valign="top">
<a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/nearby-nook-local-discovery/main/docs/screenshots/nearby-nook-map-results.png" alt="Actual Nearby Nook map and place search screenshot" width="100%" /></a>
<h3>02 — Nearby Nook</h3>
<p><b>Local discovery &amp; resilient APIs</b></p>
<p>A neighborhood explorer built with interactive maps and an API between the browser and OpenStreetMap services.</p>
<p><sub><b>Engineering:</b> Validated inputs, caching, rate limits, provider failover, and modular tests.</sub></p>
<p><a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery"><b>Source code</b></a> · <a href="https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/docs/architecture.md">Architecture</a></p>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard/main/assets/screenshots/dashboard-dark.png" alt="Actual Storefront Admin inventory dashboard screenshot" width="100%" /></a>
<h3>03 — Storefront Admin</h3>
<p><b>Inventory management &amp; backend fundamentals</b></p>
<p>An authenticated full-stack dashboard for managing product records and understanding stock levels.</p>
<p><sub><b>Engineering:</b> Express REST endpoints, MySQL, signed sessions, password verification, and validation.</sub></p>
<p><a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard"><b>Source code</b></a> · <a href="https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard#api-routes">API routes</a></p>
</td>
<td width="50%" valign="top">
<a href="https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot"><img src="https://raw.githubusercontent.com/ailevated-randy-alonzo/jobpilot-career-copilot/main/docs/screenshots/jobpilot-dashboard.png" alt="Actual JobPilot applications dashboard screenshot" width="100%" /></a>
<h3>04 — JobPilot</h3>
<p><b>AI-assisted career workflows</b></p>
<p>An application tracker with private résumé storage and role analysis grounded in a person's actual experience.</p>
<p><sub><b>Engineering:</b> Server-side OpenAI API calls, structured outputs, authenticated APIs, D1/R2 storage.</sub></p>
<p><a href="https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot"><b>Source code</b></a> · <a href="https://github.com/ailevated-randy-alonzo/jobpilot-career-copilot/tree/main/docs/screenshots">Product tour</a></p>
</td>
</tr>
</table>

<sub><b>Scope notes:</b> Hyrvanta is a portfolio-ready working release; some production integrations require configuration. JobPilot's hosted workspace is private and supports local demonstration. The linked READMEs explain setup and current limitations.</sub>

**Other builds:** [Personal portfolio](https://github.com/ailevated-randy-alonzo/randy-alonzo-portfolio) · [AILEVATED AI learning platform](https://github.com/ailevated-randy-alonzo/ailevated-ai-platform)

---

## Inside the engineering

A project is more than its UI. These are implementation details you can inspect directly:

| Decision / concern | Where to look |
|:--|:--|
| **Auth & data ownership** — keep private records scoped to their owner | [Hyrvanta security model](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/blob/main/docs/security.md) |
| **External service reliability** — validate, cache, retry, and fail transparently | [Nearby Nook gateway design](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/docs/architecture.md) |
| **API and data flows** — make CRUD operations clear and validated | [Storefront Admin implementation](https://github.com/ailevated-randy-alonzo/fullstack-ecommerce-dashboard/blob/main/server.js) |
| **Verification** — tests, type checks, and rendered-page checks | [Hyrvanta test suite](https://github.com/ailevated-randy-alonzo/hyrvanta-career-intelligence/tree/main/tests) · [Nearby Nook gateway test](https://github.com/ailevated-randy-alonzo/nearby-nook-local-discovery/blob/main/server/osmGateway.test.js) |

I distinguish a **working project release** from a production deployment. These repositories show implementation and design choices, not claims of large-scale traffic, uptime guarantees, or professional seniority.

## Tools I work with

<p>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
  <img src="https://img.shields.io/badge/JavaScript-D9AE35?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript"/>
  <img src="https://img.shields.io/badge/React-149ECA?style=flat-square&logo=react&logoColor=white" alt="React"/>
  <img src="https://img.shields.io/badge/Node.js-43853D?style=flat-square&logo=node.js&logoColor=white" alt="Node.js"/>
  <img src="https://img.shields.io/badge/Express-334155?style=flat-square&logo=express&logoColor=white" alt="Express"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL"/>
  <img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare"/>
  <img src="https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white" alt="Vitest"/>
</p>

| Area | Experience demonstrated |
|:--|:--|
| **Web & backend** | React, TypeScript, JavaScript, Node.js, Express, REST APIs |
| **Data & cloud** | MySQL, SQL, Cloudflare Workers, D1, R2, Drizzle ORM |
| **Engineering practices** | Git/GitHub, test automation, input validation, authentication, authorization |
| **Systems & IT** | Windows, Microsoft 365, network troubleshooting, incident documentation |

## Background

**Atos — IT Support Specialist**  
First-line troubleshooting, escalation, incident documentation, and support workflows.

**Technological University of the Philippines–Manila**  
Bachelor of Science in Information Technology — in progress.

**AILEVATED — Founder**  
Hands-on technology education, software projects, AI workflows, and digital resources.

---

## Let's connect

Whether you're reviewing my engineering work, considering me for a role, or discussing a project, I welcome a technical conversation.

| Professional | Community & client work |
|:--|:--|
| [✉️ Email — randyalonzo101@gmail.com](mailto:randyalonzo101@gmail.com) | [🎨 Fiverr — AILEVATED](https://www.fiverr.com/sellers/ailevated/) |
| [🌐 Personal portfolio](https://portfolio.randyalonzo101.workers.dev) | [💼 Upwork — freelancer profile](https://www.upwork.com/freelancers/~01e817b1de0c60f604?viewMode=1&mp_source=share) |
| [💼 LinkedIn — Randy M. Alonzo](https://www.linkedin.com/in/randy-m-alonzo/) | [☁️ AWS Builder — badges](https://builder.aws.com/community/@ranbyruz?tab=badges) |
| [🐙 GitHub — source repositories](https://github.com/ailevated-randy-alonzo) | [🚀 AILEVATED](https://ailevated.tech) · [▶ YouTube](https://www.youtube.com/@ailevated) |

<div align="center">
  <sub>Built around real projects, clear engineering decisions, and room to keep improving.</sub>
</div>
