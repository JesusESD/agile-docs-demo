# Helios Payments — Agile Documentation Space

This repository is the **single source of truth** for the Helios Payments Platform agile team: epics, user stories, business requirements (BRDs), release notes, sprint reports, meeting notes, and reusable templates.

It is a **demo** built to show how GitHub can replace Confluence for team documentation. Everything here is fictional sample content.

## Three ways to read this documentation

| Surface | What it is | Best for |
|---------|-----------|----------|
| **Published site (GitHub Pages)** | The `/docs` folder rendered as a searchable website with navigation, themes, and diagrams via MkDocs Material. | Day-to-day reading by the whole team and stakeholders. This is the Confluence-like experience. |
| **Repo Markdown** | The raw `.md` files in `/docs`, browsable directly on GitHub. | Editing, reviewing changes, linking from pull requests and issues. |
| **Wiki** | Lightweight pages in the `/wiki` folder, pushed to the repo Wiki. | Glossary, team norms, quick reference — content that doesn't need review workflow. |

## How editing works

Documentation is written in **Markdown** and changed through the normal GitHub flow (branch → edit → pull request → review → merge). Non-technical team members can do all of this **in the browser** — no Git knowledge required. See [`CONTRIBUTING.md`](CONTRIBUTING.md).

Once a change is merged to `main`, a **GitHub Action** rebuilds and republishes the site automatically in about a minute.

## Repository layout

```
docs/                 # All published documentation (becomes the website)
  epics/              # Epic definitions
  stories/            # User stories
  brds/               # Business Requirements Documents
  release-notes/      # Per-release notes
  reports/            # Sprint reviews & retrospectives
  meeting-notes/      # PI planning, ceremonies, decisions
  doc-templates/          # Copy-paste templates for every doc type
wiki/                 # Wiki pages (glossary, team norms)
mkdocs.yml            # Site configuration (navigation, theme)
.github/workflows/    # Auto-deploy the site to GitHub Pages
CONTRIBUTING.md       # How the agile team writes & edits docs
```

## Preview the site locally (optional, for maintainers)

```bash
pip install -r requirements.txt
mkdocs serve
# open http://127.0.0.1:8000
```

## Roll-out note (free vs Enterprise)

This demo runs on a **public** repository because GitHub Wiki and Pages require a paid plan to work on **private** repos. On **GitHub Enterprise Cloud**, the identical setup runs on a **private** repo with no changes — see `../CONFLUENCE-VS-GITHUB.md` and `../DEMO-GUIDE.md` at the root of the delivery folder.
