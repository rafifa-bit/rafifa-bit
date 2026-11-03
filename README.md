<img src="assets/diablo-cabecalho.svg" width="100%" alt="Rafael Vieira, tech lead and full-stack developer in Belém, Brazil. Open to remote work. Stay awhile and listen: I build what teams run on.">

I build the software that runs [NÓS Soluções Sustentáveis](https://nossustentaveis.com), a company that supports family-farming cooperatives in the Amazon. The tech team is two people, so I design, code, review, deploy, and sit with the people who use it.

The code is private, so here is what it does and how I built it.

### ▶ Quest log

<p>
<img src="assets/diablo-erp.svg" width="49%" alt="ERP NÓS, unique system: six modules, one database schema each, tested business rules. Built from October 2026.">
<img src="assets/diablo-ia.svg" width="49%" alt="AI reader, rare scroll: reads scanned contracts, 30 of 30 items matched, checked by a person.">
</p>
<p>
<img src="assets/diablo-painel.svg" width="49%" alt="Dashboard, set item: one screen, cross filters, shareable links, with a map of the state.">
<img src="assets/diablo-relatorios.svg" width="49%" alt="Reports, magic tome: one-click export to Word and Excel with the same charts as the screen, on brand.">
</p>

**ERP NÓS.** Built from zero starting October 2026: requests, finance, projects, field survey and an executive dashboard. Each module has its own Postgres schema, and business rules are pure functions with their own tests. Every screen follows the company's design system and is checked from 320px to 1920px wide.

**AI contract reading.** Reads government food contracts, scanned PDFs included, and fills in buyer, products, quantities and prices. Every line is cross-checked (quantity × price = total) and a person confirms it on screen. It switches between models when one is overloaded. Paid billing comes before the first outside client, because contracts carry personal IDs.

**Strategic dashboard.** Power BI-style: a map of the state, production, seasonality and public-policy reach. It fits on one screen (tested at 1280×720), and clicking anything filters everything. Partner institutions get shareable branded links, with exports to PDF, Excel and Word.

**Branded reports.** One click makes a Word report that follows the company's document manual, plus a spreadsheet with one tab per theme and the image of each chart. Field spreadsheets go in through the API with idempotency keys, so running the import twice never duplicates a record.

**Next level:** turning the contracts module into a SaaS product for cooperatives that sell to Brazil's national school-meals program (PNAE). Pricing tiers, data-ownership rules under Brazil's privacy law (LGPD) and the competition are already mapped.

### ▶ How I ship

<img src="assets/diablo-masmorra.svg" width="100%" alt="Dungeon levels, how I ship: prototype users approve, a branch per task, review by the second developer, staging first, release after the OK.">

- **Rules in plain language.** Business rules are written so the people who use the system can read them, and they have tests.
- **Incidents become rules.** I once deployed the API before its database migration and every shared link returned an error. Now I check the data right after any deploy that has a migration. When a missing storage bucket broke file uploads in staging, the fix made the API create the bucket itself.
- **AI coding agents as a pair.** I write the brief, review every diff, and keep a reviewer agent that challenges plans before any code is written.
- **Simple screens.** Interfaces that people without a tech background can use on day one, with no decoration for its own sake.

### ▶ Inventory

<img src="assets/diablo-inventario.svg" width="100%" alt="Inventory. Equipped: TypeScript, React, Vite, Cloudflare Workers, Supabase, PostgreSQL, Drizzle ORM, pnpm, Vitest, Gemini API. Stash: Python, Playwright, pandas, Streamlit, Plotly, Next.js, YOLO, Roboflow.">

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

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Rafael_Vieira-1a1c2c?style=for-the-badge&logo=linkedin&logoColor=a7f070)](https://www.linkedin.com/in/rafael-vieiras)
[![Email](https://img.shields.io/badge/Email-rafael.baiaravi11%40gmail.com-1a1c2c?style=for-the-badge&logo=gmail&logoColor=ffcd75)](mailto:rafael.baiaravi11@gmail.com)

Portuguese (native) | English (basic, improving)
