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
- `assets/resume/gabriel-franco-data-engineer-resume-en.html`: editable English resume.
- `assets/resume/gabriel-franco-data-engineer-resume-en.pdf`: generated English resume PDF.
- `assets/resume/gabriel-franco-data-engineer-resume-pt-br.html`: editable Portuguese resume.
- `assets/resume/gabriel-franco-data-engineer-resume-pt-br.pdf`: generated Portuguese resume PDF.
- `career-materials/linkedin-positioning.md`: LinkedIn headline, About, experience bullets, Featured suggestions, and recruiter message templates.
- `career-materials/remote-data-engineer-roadmap.md`: certification, projects, English, GitHub workflow, and remote job roadmap.
- `career-materials/skill-proof-project-guide.md`: public sanitized guide mapping skills to certifications, portfolio projects, and evidence.

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
- SQL, Spark SQL, PySpark, Databricks, Delta Lake, Python, Apache Airflow, GitHub Actions.
- Banking data, fixed-income rules, trade finance, config-driven/metadata-driven parameterization, batch orchestration, Oracle Exadata, Delta Lake.
- Control-M remains in resume/experience as real production exposure, but public positioning should gradually move toward Apache Airflow as the modern orchestration skill.
- Open to remote data engineering opportunities.
- Career target: full remote Data Engineer roles, preferably international, growing toward mid-level readiness.

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

Current PT-BR web resume:

```text
assets/resume/gabriel-franco-data-engineer-resume-pt-br.html
```

Current PT-BR PDF resume:

```text
assets/resume/gabriel-franco-data-engineer-resume-pt-br.pdf
```

Current English web resume:

```text
assets/resume/gabriel-franco-data-engineer-resume-en.html
```

Current English PDF resume:

```text
assets/resume/gabriel-franco-data-engineer-resume-en.pdf
```

The resume PDFs are generated from the HTML resume files with Chrome headless. Chrome is installed on this machine but is not available as a simple `chrome` command in PATH.

Regenerate EN PDF:

```powershell
& "C:\Program Files\Google\Chrome\Application\chrome.exe" --headless --disable-gpu --print-to-pdf="C:\Users\gabri\OneDrive\Documentos\2026_codex\p\assets\resume\gabriel-franco-data-engineer-resume-en.pdf" "file:///C:/Users/gabri/OneDrive/Documentos/2026_codex/p/assets/resume/gabriel-franco-data-engineer-resume-en.html"
```

Regenerate PT-BR PDF:

```powershell
& "C:\Program Files\Google\Chrome\Application\chrome.exe" --headless --disable-gpu --print-to-pdf="C:\Users\gabri\OneDrive\Documentos\2026_codex\p\assets\resume\gabriel-franco-data-engineer-resume-pt-br.pdf" "file:///C:/Users/gabri/OneDrive/Documentos/2026_codex/p/assets/resume/gabriel-franco-data-engineer-resume-pt-br.html"
```

The portfolio section currently links to:

- EN resume: HTML page with an internal PDF download button.
- PT-BR resume: HTML page with an internal PDF download button.

If replacing resume files, keep the same filenames when possible so the site links do not break.

## Project Section Policy

Be honest about project status.

Currently active:

- Certification Simulator App: active prototype.

Roadmap/study areas:

- Lakehouse Engineering.
- Workflow Orchestration.

Do not describe unbuilt projects as completed portfolio projects. When a project gets real code and documentation, then update this section with the repository link and concrete technical details.

## Private Context Policy

Private career context and raw PDI notes are stored outside this public repository at:

```text
C:\Users\gabri\OneDrive\Documentos\2026_codex\private_career_context
```

Latest private career context:

```text
C:\Users\gabri\OneDrive\Documentos\2026_codex\private_career_context\trajetoria-dados-financeiros-2026-06-18.md
```

Do not copy that folder into this repository or publish it.

Before publishing career text, sanitize it:

- Remove internal system names, private links, manager names, internal library names, and internal product codes.
- Keep market-recognized terms such as CRA, CRI, debentures, trade finance, Control-M, Databricks, Delta Lake, Oracle/Exadata, GitHub Actions, config-driven, and metadata-driven.
- Keep Control-M as real work experience, but do not overemphasize it as Gabriel's target brand.
- Keep Airflow as certification/project skill until Gabriel has real work experience with it.

Sanitized translations:

- Internal financial data platform instead of internal system names.
- Metadata-driven parameterizations instead of internal table/control names.
- Corporate pipeline orchestrator instead of internal scheduler names when needed.
- Financial unit value calculation instead of proprietary demand names.
- Internal pipeline framework instead of internal framework names.
- Schema validation and parameterization front instead of internal front/version names.

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

## Handoff Policy

For every repository we create, edit, or publish from now on, keep a `HANDOFF.md` file updated.

The handoff should include:

- Project purpose and current status.
- Main files and folder structure.
- Local setup and run commands.
- Deploy/publish instructions.
- Important links, credentials policy, and environment variables without secrets.
- Known issues, decisions made, and next steps.
- What changed in the latest meaningful work session.

When changing a project, update `HANDOFF.md` in the same commit whenever the change affects setup, deploy, structure, links, roadmap, or continuation context.

## GitHub Workflow Policy

Going forward, meaningful changes should preferably use a professional GitHub workflow:

1. Create an issue.
2. Create a branch.
3. Commit to the branch.
4. Open a pull request.
5. Include what changed, why, and how to test.
6. Merge the PR.
7. Close the issue.

Small emergency fixes can still be committed directly, but portfolio/project work should use issues and PRs to build visible evidence of collaboration-ready habits.

## Next Improvements

- Keep both HTML resumes and generated PDFs in sync.
- Keep `career-materials/skill-proof-project-guide.md` aligned with project execution.
- Add the real `simu_app` repository link once it is ready to be public.
- Update LinkedIn using `career-materials/linkedin-positioning.md`.
- Follow the certification/project roadmap in `career-materials/remote-data-engineer-roadmap.md`.
- Improve visual validation in a normal browser after each UI change.
- Add screenshots or a simple Open Graph image later.
- Consider moving CSS into `styles.css` if the single-file HTML becomes hard to maintain.
