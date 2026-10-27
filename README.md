# 🚇 The Databricks Line

**An interactive, hands-on roadmap to the Databricks platform, designed like a metro map.**

Sixteen stops across five lines, from your first notebook to AI agents. Each stop explains one part of Databricks in plain English, translates it into the industry term you already know, and lets you try a small task that feels like working in a real workspace.

No login. No install. No cost. Works on your phone.

**▶ [Ride the line](https://<your-username>.github.io/databricks-line/)**

<p align="center">
  <img src="assets/demo.gif" alt="Demo: tapping through the metro map, running a notebook, restoring a Delta table, granting access in Unity Catalog, building a pipeline and asking Genie a question" width="320">
</p>

---

## Contents

- [Why this exists](#why-this-exists)
- [The map](#the-map)
- [What you can do at each stop](#what-you-can-do-at-each-stop)
- [Features](#features)
- [Getting started](#getting-started)
- [Publishing your own copy with GitHub Pages](#publishing-your-own-copy-with-github-pages)
- [Project structure](#project-structure)
- [How it's built](#how-its-built)
- [Customising the content](#customising-the-content)
- [Accessibility](#accessibility)
- [Browser support](#browser-support)
- [Contributing](#contributing)
- [Disclaimer](#disclaimer)
- [License](#license)
- [Author](#author)

---

## Why this exists

Many people still think of Databricks as "the place where Spark transformations run". Today it covers the whole data lifecycle: ingestion, transformation, orchestration, warehousing, dashboards, natural-language analytics, machine learning, AI agents, data sharing and operational databases, all under one governance layer.

Reading documentation is a slow way to build that mental model. The Databricks Line lets people **learn by doing**: each concept comes with a two-minute task that shows how the feature behaves, using sample data in the browser.

It's built for:

- **Newcomers** who have never opened a Databricks workspace
- **Data professionals** coming from other tools, such as Azure Data Factory (ADF), Airflow, Snowflake or Power BI, who want to map what they know onto Databricks
- **Teams and trainers** who need a friendly, shareable introduction for onboarding

---

## The map

| Line | Stops |
|---|---|
| 🟢 **Foundations** | Workspace and notebooks · Delta Lake tables · Unity Catalog · Compute |
| 🟡 **Data engineering** | Lakeflow Connect · Declarative pipelines and Designer · Lakeflow Jobs |
| 🔵 **Analytics** | Databricks SQL · AI/BI dashboards · Genie |
| 🟠 **AI** | Genie Code · MLflow and Model Serving · AI agents |
| 🟣 **Run the business** | Sharing and Marketplace · Lakebase and Apps · Observability and cost |

Every stop pairs the Databricks name with its **industry term**:

| Databricks | Industry term |
|---|---|
| Workspace and notebooks | Collaborative development environment |
| Delta Lake | Open table format with ACID (atomicity, consistency, isolation, durability) transactions |
| Unity Catalog | Data catalog and governance |
| Compute | Compute engine: clusters and serverless |
| Lakeflow Connect | Data ingestion and CDC (change data capture) connectors |
| Declarative pipelines and Designer | ETL (extract, transform, load) and data transformation |
| Lakeflow Jobs | Workflow orchestration |
| Databricks SQL | Data warehouse |
| AI/BI dashboards | Business intelligence (BI) and visualisation |
| Genie | Conversational analytics |
| Genie Code | AI coding assistant |
| MLflow and Model Serving | MLOps: machine learning lifecycle |
| AI agents | Generative and agentic AI |
| Sharing and Marketplace | Data sharing and data exchange |
| Lakebase and Apps | Operational database (OLTP, online transaction processing) and internal apps |
| Observability and cost | Monitoring, audit and FinOps (cloud financial operations) |

A searchable **Terms** page translates 34 industry terms into their Databricks equivalents.

---

## What you can do at each stop

| # | Stop | Hands-on task |
|---|---|---|
| 1 | Workspace and notebooks | Create a notebook, pick a language and run your first cell |
| 2 | Delta Lake tables | Slide through a table's version history and restore it after a bad update |
| 3 | Unity Catalog | Browse the catalog, grant read access to a group, then view the data as an analyst with emails masked |
| 4 | Compute | Match three workloads to serverless, a classic cluster or a SQL warehouse |
| 5 | Lakeflow Connect | Ingest from Salesforce, SQL Server, files in storage or Kafka |
| 6 | Declarative pipelines | Build a bronze → silver → gold pipeline and switch on a data quality rule to catch bad rows |
| 7 | Lakeflow Jobs | Pick a trigger, run a job, watch a task fail, then fix it with a repair run |
| 8 | Databricks SQL | Run queries in a SQL editor and get tables and charts back |
| 9 | AI/BI dashboards | Choose a measure, chart type and region filter, then publish |
| 10 | Genie | Ask questions in plain English and see the SQL behind each answer |
| 11 | Genie Code | Watch a pipeline get written from a one-line prompt, then accept and run it |
| 12 | MLflow and Model Serving | Pick the best experiment run, register it, serve it and get live predictions |
| 13 | AI agents | Assemble an agent from knowledge, tools and guardrails, then ask it a question |
| 14 | Sharing and Marketplace | Share a table with a partner, with a warning if you pick personal data |
| 15 | Lakebase and Apps | Save orders from an app into Postgres, then sync them to the lakehouse |
| 16 | Observability and cost | Query billing system tables and set a budget alert |

Wrong choices give a hint, not just a red cross, so people learn why the right answer is right.

---

## Features

- 🗺️ **Metro-map navigation** with colour-coded lines and stops that fill in as you complete them
- 💡 **Learn and Try it tabs** at every stop: an everyday analogy, key points, familiar comparable tools and a hands-on task
- 🔁 **Industry term translation** on every stop, plus a searchable glossary
- 🏅 **Journey page** with a badge for each line and an Explorer's pass stamped with your name when all 16 stops are complete
- 📱 **Mobile first**: full-screen stops on phones, swipe between stops, a bottom tab bar and large tap targets
- ⌨️ **Keyboard friendly**: arrow keys move between stops and Escape closes a stop
- 🌗 **Light and dark themes** that follow your device, with a manual toggle
- 📦 **One self-contained file** with no build step, no framework and no tracking

---

## Getting started

### Use it online

Open the live page: **https://\<your-username\>.github.io/databricks-line/**

### Run it locally

The whole app is a single HTML file.

```bash
git clone https://github.com/<your-username>/databricks-line.git
cd databricks-line
```

Then either double-click `index.html`, or serve the folder:

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

Everything works offline. Fonts load from Google Fonts when you're online and fall back to standard system fonts when you're not.

---

## Publishing your own copy with GitHub Pages

1. Create a new **public** repository, for example `databricks-line`.
2. Upload `index.html` (and the `assets` folder if you want the demo GIF in your README).
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, then select **Save**.
5. After a minute or two, your page is live at `https://<your-username>.github.io/databricks-line/`.

Replace `<your-username>` in this README with your GitHub username so the links work.

> **Tip:** if you just want a quick public link without GitHub, drag `index.html` onto [Netlify Drop](https://app.netlify.com/drop).

---

## Project structure

```
databricks-line/
├── index.html        # The entire app: markup, styles, icons, content and logic
├── assets/
│   ├── demo.gif      # Animated walkthrough used in this README
│   └── demo.mp4      # Higher-quality video version for social posts
├── LICENSE.md
└── README.md
```

---

## How it's built

| Part | Approach |
|---|---|
| Stack | Plain HTML, CSS and JavaScript. No frameworks, no dependencies, no build tools |
| Icons | Custom inline SVG (Scalable Vector Graphics) symbols, so they're crisp at any size and work offline |
| Charts | Hand-drawn SVG bar and line charts generated from the sample data |
| Theming | CSS (Cascading Style Sheets) custom properties with separate light and dark palettes |
| Data | A small sample retail dataset held in memory; every task runs entirely in your browser |
| State | In memory only. Progress resets when the page reloads, and nothing is stored or sent anywhere |
| Fonts | Lora for headings, Source Sans 3 for text and Source Code Pro for code, with system fallbacks |

---

## Customising the content

All content lives in `index.html`, inside the `<script>` block near the bottom.

| To change | Edit |
|---|---|
| Lines (name, colour, description) | The `ZONES` array |
| Stops (name, industry term, analogy, key points, comparable tools, task title) | The `S` array |
| Glossary terms | The `GLOSS` array: `[industry term, Databricks name, description, stop id]` |
| Sample data | The `ORDERS` array |
| A stop's hands-on task | The matching function in the `TASKS` object, keyed by stop id |

To add a stop:

1. Add an entry to `S` with a unique `id` and the `z` (line) it belongs to.
2. Add a function with the same `id` to `TASKS`. It receives the task container element and an `ok` callback. Call `ok()` when the user completes the task.
3. Optionally add glossary entries pointing to the new `id`.

Colours are defined once as CSS variables at the top of the file (`--teal`, `--gold`, `--steel`, `--bronze`, `--plum` and their light tints), with matching dark-mode values.

---

## Accessibility

- Semantic headings, landmarks and a labelled dialog for each stop
- Visible keyboard focus on every interactive element
- All controls reachable by keyboard; Escape closes a stop, arrow keys move between stops
- Status messages announced through a live region
- Motion respects the **reduce motion** system setting
- Colour is never the only signal: completed stops also show a tick, and feedback is always written out

If you find an accessibility issue, please [open an issue](../../issues).

---

## Browser support

Works in current versions of Chrome, Edge, Safari and Firefox on desktop and mobile, including iOS (iPhone and iPad) and Android. Tested at screen widths from 320 px (small phones) up to desktop.

---

## Contributing

Suggestions and fixes are welcome.

1. Fork the repository.
2. Create a branch: `git checkout -b improve-stop-genie`.
3. Make your changes in `index.html` and test them on both a phone-sized and a desktop-sized window.
4. Open a pull request describing what you changed and why.

Good first contributions:

- A new hands-on task or a clearer analogy for an existing stop
- Additional glossary terms
- Translations
- Accessibility improvements

Because Databricks evolves quickly, corrections that bring a stop in line with the latest [official documentation](https://docs.databricks.com/) are especially appreciated.

---

## Disclaimer

The Databricks Line is an **independent, unofficial learning project**. It is not affiliated with, endorsed by or sponsored by Databricks, Inc.

- All tasks are **simulations** that run in your browser with made-up sample data. Nothing connects to a real Databricks workspace or account.
- The SQL shown is realistic and illustrative; results, ML (machine learning) predictions and agent answers are pre-built for teaching purposes.
- Feature names and availability change over time and vary by cloud, region and release stage. Always check the [official Databricks documentation](https://docs.databricks.com/) before relying on a feature.

Databricks, Delta Lake, Unity Catalog, MLflow, Lakeflow, Genie and related names are trademarks of their respective owners and are used here only to describe the products being taught.

---

## License

Released under the [MIT License](LICENSE.md). You're free to use, adapt and share it, including for training and onboarding, as long as the copyright notice is kept.

---

## Author

**Vijini Tennekoon**

If this helped you understand Databricks a little better, a ⭐ on the repository helps others find it.
