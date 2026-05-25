# Handoff - Gabriel Franco Portfolio

## Project

Repository: `GabrieloFranco/portfolio`

Published site: `https://gabrielofranco.github.io/portfolio/`

Purpose: static portfolio website for Gabriel Franco, focused on Data Engineering positioning for international opportunities.

## Current State

The repository was rebuilt from an old 2023 portfolio into a clean static site.

Current important files:

- `index.html`: full one-page portfolio with embedded CSS.
- `README.md`: short repository description and deployment notes.
- `HANDOFF.md`: this continuation guide.
- `assets/resume/gabriel-franco-data-engineer-resume-pt-br.pdf`: downloadable/viewable resume.

The previous repository contained duplicated folders, old pages, large generated images, and executable files. Those were removed intentionally.

## Deployment

GitHub Pages is enabled.

Source:

- Branch: `master`
- Path: `/`

After pushing to `master`, GitHub Pages should rebuild automatically.

Useful command:

```powershell
& "C:\Users\gabri\OneDrive\Documentos\2026_codex\tools\bin\gh.exe" api repos/GabrieloFranco/portfolio/pages
```

Expected site URL:

```text
https://gabrielofranco.github.io/portfolio/
```

## Design Direction

The site should feel professional, calm, and credible for a Data Engineer.

Current positioning:

- Data Engineer in financial data platforms.
- SQL, PySpark, Databricks, Delta Lake, Python, Control-M.
- Banking data, fixed-income rules, batch orchestration, Oracle Exadata, Delta Lake.
- Open to remote data engineering opportunities.

Avoid making the site look like a student landing page or a generic full-stack portfolio.

## Contact Links

Email:

```text
mailto:ds.gabrielfranco@gmail.com?subject=Data%20Engineering%20Opportunity&body=Hi%20Gabriel%2C%20I%20saw%20your%20profile%20and%20would%20like%20to%20talk.
```

WhatsApp:

```text
https://wa.me/5511958814398?text=Hi%20Gabriel%2C%20I%20saw%20your%20profile%20and%20would%20like%20to%20talk.
```

LinkedIn:

```text
https://www.linkedin.com/in/gabrielofranco
```

GitHub:

```text
https://github.com/GabrieloFranco
```

## Resume

Resume section is linked from the top navigation.

Current PDF:

```text
assets/resume/gabriel-franco-data-engineer-resume-pt-br.pdf
```

If replacing the resume, keep the same filename when possible so the site link does not break.

## Project Section Policy

Be honest about project status.

Currently active:

- Certification Simulator App: active prototype.

Roadmap/study areas:

- Lakehouse Engineering.
- Workflow Orchestration.

Do not describe unbuilt projects as completed portfolio projects. When a project gets real code and documentation, then update this section with the repository link and concrete technical details.

## Local Workflow

From the local clone:

```powershell
cd C:\Users\gabri\OneDrive\Documentos\2026_codex\p
git status
```

Commit and push:

```powershell
git add -A
git commit -m "Describe the portfolio change"
git push origin master
```

In this environment, if Git reports a safe-directory issue, use:

```powershell
git -c safe.directory="C:/Users/gabri/OneDrive/Documentos/2026_codex/p" status
```

## Next Improvements

- Add an English resume version and link both PT-BR and EN-US.
- Add the real `simu_app` repository link once it is ready to be public.
- Improve visual validation in a normal browser after each UI change.
- Add screenshots or a simple Open Graph image later.
- Consider moving CSS into `styles.css` if the single-file HTML becomes hard to maintain.

