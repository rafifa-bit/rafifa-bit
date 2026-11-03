<img src="assets/diablo-cabecalho.svg" width="100%" alt="Rafael Vieira, tech lead and full-stack developer in Belém, Brazil. Open to remote work. Stay awhile and listen: I build what teams run on.">

I build the software that runs [NÓS Soluções Sustentáveis](https://nossustentaveis.com), a company that supports family-farming cooperatives in the Amazon. The tech team is two people, so I design, code, review, deploy, and sit with the people who use it. I also build AI features with the Claude and Gemini APIs: document reading and AI-generated dashboards and reports.

<a href="https://elo.nossustentaveis.com"><img src="https://img.shields.io/badge/ERP_N%C3%93S-elo.nossustentaveis.com-d4a84a?style=for-the-badge&labelColor=0b0a0d" alt="ERP NÓS: elo.nossustentaveis.com"></a>
<a href="https://nossustentaveis.com"><img src="https://img.shields.io/badge/N%C3%93S-nossustentaveis.com-b3261e?style=for-the-badge&labelColor=0b0a0d" alt="NÓS Soluções Sustentáveis: nossustentaveis.com"></a>

The code is private (the ERP needs a login), so here is what it does and how I built it.

### ▶ Quest log

<p>
<a href="https://elo.nossustentaveis.com"><img src="assets/diablo-erp.svg" width="49%" alt="ERP NÓS, unique system: six modules, one database schema each, tested business rules. Built from October 2026."></a>
<a href="https://elo.nossustentaveis.com"><img src="assets/diablo-ia.svg" width="49%" alt="AI reader, rare scroll: reads scanned contracts, 30 of 30 items matched, checked by a person."></a>
</p>
<p>
<a href="https://elo.nossustentaveis.com"><img src="assets/diablo-painel.svg" width="49%" alt="Dashboard, set item: one screen, cross filters, shareable links, with a map of the state."></a>
<a href="https://elo.nossustentaveis.com"><img src="assets/diablo-relatorios.svg" width="49%" alt="AI reports, magic tome: 29 charts, commentary written with the Claude API, every number checked, exported to Word and Excel."></a>
</p>

**[ERP NÓS](https://elo.nossustentaveis.com).** Built from zero starting October 2026: requests, finance, projects, field survey and an executive dashboard. Each module has its own Postgres schema, and business rules are pure functions with their own tests. Every screen follows the company's design system and is checked from 320px to 1920px wide.

**AI document reading (Gemini API).** Reads government food contracts, scanned PDFs included, and fills in buyer, products, quantities and prices. Every line is cross-checked (quantity × price = total) and a person confirms it on screen. It switches between models when one is overloaded. Paid billing comes before the first outside client, because contracts carry personal IDs.

**AI-generated dashboards and reports (Claude API).** A cooperative survey spreadsheet goes in. A dashboard with 29 charts and a Word report come out, following the company's document manual, plus a spreadsheet with the image of each chart. The Claude API writes the commentary for every chart from facts already calculated, and each number it cites is checked against the data. If it invents a number, the text is requested again. On a second miss, an automatic text built only from correct numbers is used.

**Strategic dashboard.** Power BI-style: a map of the state, production, seasonality and public-policy reach. It fits on one screen (tested at 1280×720), and clicking anything filters everything. Partner institutions get shareable branded links, with exports to PDF, Excel and Word. Field spreadsheets go in through the API with idempotency keys, so running the import twice never duplicates a record.

**Next level:** turning the contracts module into a SaaS product for cooperatives that sell to Brazil's national school-meals program (PNAE). Pricing tiers, data-ownership rules under Brazil's privacy law (LGPD) and the competition are already mapped.

### ▶ How I ship

<img src="assets/diablo-masmorra.svg" width="100%" alt="Dungeon levels, how I ship: prototype users approve, a branch per task, review by the second developer, staging first, release after the OK.">

- **Rules in plain language.** Business rules are written so the people who use the system can read them, and they have tests.
- **Incidents become rules.** I once deployed the API before its database migration and every shared link returned an error. Now I check the data right after any deploy that has a migration. When a missing storage bucket broke file uploads in staging, the fix made the API create the bucket itself.
- **AI coding agents as a pair.** I write the brief, review every diff, and keep a reviewer agent that challenges plans before any code is written.
- **Simple screens.** Interfaces that people without a tech background can use on day one, with no decoration for its own sake.

### ▶ Inventory

<img src="assets/diablo-inventario.svg" width="100%" alt="Inventory. Equipped: TypeScript, React, Vite, Cloudflare Workers, Supabase, PostgreSQL, Drizzle ORM, pnpm, Vitest, Claude API, Gemini API. Stash: Python, Playwright, pandas, Streamlit, Plotly, Next.js, YOLO, Roboflow.">

### ▶ Previous levels

- **Public sector (State Department of Education of Pará):** Python automation and data dashboards for HR and administrative processes, and a web app to track retirement cases (Next.js, Supabase, LLM-assisted data import).
- **Computer vision:** detecting ID documents with YOLO models, and a face-recognition sign-in prototype.

### ▶ Contributions

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/rafifa-bit/rafifa-bit/output/snake-dark.svg">
  <img src="https://raw.githubusercontent.com/rafifa-bit/rafifa-bit/output/snake-light.svg" width="100%" alt="A snake eating the squares of my contribution graph.">
</picture>

### ▶ Contact

<a href="https://www.linkedin.com/in/rafael-vieiras"><img src="assets/diablo-start.svg" width="100%" alt="Press start to hire: contact Rafael on LinkedIn."></a>

[![NÓS](https://img.shields.io/badge/N%C3%93S-nossustentaveis.com-0b0a0d?style=for-the-badge&logoColor=d4a84a)](https://nossustentaveis.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Rafael_Vieira-1a1c2c?style=for-the-badge&logo=linkedin&logoColor=a7f070)](https://www.linkedin.com/in/rafael-vieiras)
[![Email](https://img.shields.io/badge/Email-rafael.baiaravi11%40gmail.com-1a1c2c?style=for-the-badge&logo=gmail&logoColor=ffcd75)](mailto:rafael.baiaravi11@gmail.com)

Portuguese (native) | English (basic, improving)
