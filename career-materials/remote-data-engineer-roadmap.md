# Remote Data Engineer Roadmap - Gabriel Franco

Goal: move from hybrid work to full remote Data Engineering roles, preferably international, while building evidence for mid-level readiness.

## Current Positioning

Current strengths:

- Real banking data experience.
- SQL, Spark SQL, Python, PySpark, Databricks, Delta Lake.
- Financial data pipelines, fixed-income rules, trade finance, and business-facing delivery.
- Config-driven/metadata-driven parameterization experience.
- Oracle/Exadata integration exposure.
- Batch orchestration, monitoring, and troubleshooting with Control-M as the current production base.
- Active transition path from Control-M concepts to Apache Airflow for public portfolio and market positioning.
- Power BI and data analyst background.
- Public GitHub and portfolio aligned with Data Engineering.

Current gaps:

- English is not yet comfortable enough for international interviews.
- Public portfolio still has few real Data Engineering projects.
- CI/CD and GitHub Actions need stronger practical proof.
- Airflow is the target orchestration brand, but still needs certification and a demonstrated public project.
- Need more visible evidence of mid-level engineering behavior: issues, branches, PRs, docs, tests, and deployable examples.

## Career Strategy

The target is:

- Full remote.
- Data Engineer.
- Junior strong to mid-level.
- Stack close to SQL, Python, PySpark, Databricks, Delta Lake, Apache Airflow, GitHub Actions, and cloud data platforms.

Do not overclaim seniority. The strategy is to show:

- Production exposure.
- Strong learning velocity.
- Clear technical roadmap.
- Professional GitHub workflow.
- Real projects that prove readiness.

## Certification Order

### 0. Immediate Sprint - Databricks Certified Data Engineer Associate

Priority: highest right now.

Why:

- Directly matches current work.
- Strong signal for Databricks/PySpark roles.
- Helps organize existing knowledge.
- Should connect to the first portfolio project.

Evidence to produce:

- Study notes.
- Practice questions in `simu_app`.
- Databricks/PySpark portfolio project.

If an exam attempt is planned for the current week, keep the week focused on Databricks and avoid splitting deep study time across other certifications.

### 1. AZ-900 - Microsoft Azure Fundamentals

Priority: high after the immediate Databricks sprint.

Why:

- Low-friction Azure credential.
- Helps with cloud vocabulary for international interviews.
- Makes DP-750 easier by covering core Azure concepts first.

Evidence to produce:

- Short Azure fundamentals notes.
- A cloud glossary connected to Databricks and Data Engineering.

### 2. Microsoft DP-750 - Azure Databricks Data Engineer Associate

Priority: high after AZ-900 and/or Databricks Associate.

Why:

- Aligns Databricks with Azure.
- Strong international signal.
- Covers pipelines, troubleshooting, Unity Catalog, governance, SQL, Python, and SDLC/Git.

Evidence to produce:

- Azure Databricks study plan.
- Project documentation mentioning cloud/lakehouse architecture.

### 3. GitHub Actions / CI-CD

Priority: high.

Why:

- Builds CI/CD confidence quickly.
- Helps professionalize every project.
- Supports the GitHub contribution graph with issues, PRs, and workflows.

Evidence to produce:

- CI pipeline in portfolio projects.
- Lint/test workflows.
- PR workflow with issue closing.

### 4. Apache Airflow Fundamentals

Recommended option: Astronomer Certification for Apache Airflow Fundamentals.

Why:

- Airflow is more marketable than Control-M for modern Data Engineering roles.
- Good bridge from batch monitoring to workflow orchestration.
- A functional DAG is stronger evidence than a badge alone.

Evidence to produce:

- Airflow project with Docker.
- DAGs with retries, logs, schedule, dependencies, and failure handling.
- README explaining orchestration design.

### 5. GitHub Foundations

Priority: optional.

Why:

- Useful for completeness.
- Less important than GitHub Actions applied in real repos.
- Good if quick and inexpensive.

### 6. PL-300

Priority: optional.

Why:

- Useful only if Gabriel wants to keep Power BI as a stronger secondary track.
- Not the main route for Data Engineering roles.

## 90-Day Execution Plan

### Days 1-15 - Professional Surface + Databricks Sprint

Deliverables:

- LinkedIn updated with remote/international positioning.
- English and PT-BR resumes improved and published.
- GitHub profile aligned with Data Engineering.
- Portfolio public and clean.
- Databricks Associate study kit in Databricks notebooks.
- Start using issues, branches, and PRs for all future repo work.

Daily habits:

- 20 minutes English speaking practice.
- 45-90 minutes Databricks Associate study.
- 1 small GitHub note, issue, or study artifact when learning something useful.

### Days 16-45 - Databricks Associate + Portfolio Proof

Deliverables:

- Finish Databricks Associate study.
- Add certification content to `simu_app`.
- Create first real Data Engineering project.
- Add README, HANDOFF, issues, PRs, and basic CI.

Focus:

- Spark SQL and PySpark transformations.
- Databricks workflows/jobs.
- Delta Lake.
- Data validation.
- Medallion architecture.

### Days 46-70 - GitHub Actions + CI/CD

Deliverables:

- GitHub Actions study.
- Add CI to active repos.
- Use PR template and issue template.
- Create visible contribution activity beyond commits.

Focus:

- Lint/test pipeline.
- Branch workflow.
- Pull requests.
- Release notes or changelog.

### Days 71-90 - Airflow Project + Applications

Deliverables:

- Airflow + Docker project.
- DAG with real data ingestion/transformation.
- Logs, retries, schedule, and documentation.
- Start applying to remote roles.

Focus:

- DAG authoring.
- Task dependencies.
- Failure handling.
- Local development with Docker.
- Interview story in English.

## English Plan

Minimum target: functional work English, not perfect English.

Daily routine:

- 10 minutes: read one technical paragraph aloud.
- 10 minutes: explain one project out loud.
- 10 minutes: answer one interview question.

Weekly routine:

- 1 mock self-introduction.
- 1 mock project explanation.
- 1 mock behavioral answer.
- 1 written recruiter reply.

Core scripts to master:

1. Self-introduction.
2. Current work explanation.
3. Databricks/PySpark project explanation.
4. Why remote/international roles.
5. A troubleshooting story.
6. A business-stakeholder collaboration story.
7. A learning/growth story.

## GitHub Workflow Going Forward

For every meaningful change:

1. Create an issue.
2. Create a branch.
3. Commit changes.
4. Open a pull request.
5. Include a short PR description:
   - What changed.
   - Why.
   - How to test.
6. Merge the PR.
7. Close the issue.

This builds evidence for issues, pull requests, commit history, professional delivery, and documentation discipline.

## Project Roadmap

### Project 1 - Lakehouse Financial Data

Status: not started.

Goal:

- Demonstrate PySpark, Delta Lake, medallion architecture, data quality, and documentation.

Suggested scope:

- Public financial dataset, preferably BCB indicators.
- Bronze ingestion.
- Silver cleaning/standardization.
- Gold aggregations.
- Business rules.
- Tests.
- README with architecture diagram.
- HANDOFF for continuation.

### Project 2 - Python ETL + Tests + CI/CD

Status: not started.

Goal:

- Prove Python engineering quality and CI/CD basics.

Suggested scope:

- BCB API ingestion.
- Clean/normalize/aggregate data.
- Save output as Parquet/CSV.
- `pytest` tests.
- `ruff` linting.
- GitHub Actions workflow.

### Project 3 - Config-Driven SQL Pipeline

Status: not started.

Goal:

- Publicly prove the business-rule and parameterization thinking used at work, without exposing real banking data or rules.

Suggested scope:

- Fictitious financial product rules in CSV/YAML.
- Python generator that turns configuration into SQL.
- DuckDB or SQLite execution.
- Validation tests.
- README explaining config-driven/metadata-driven architecture.

### Project 4 - Airflow Batch Pipeline

Status: not started.

Goal:

- Translate Control-M experience into modern Apache Airflow orchestration proof.

Suggested scope:

- Airflow + Docker Compose.
- DAG for ingestion, validation, transformation, and reporting.
- FileSensor, retries, failure handling, dependencies, success marker, logs, and documentation.
- GitHub Actions CI.

### Project 5 - Certification Simulator App

Status: active prototype.

Goal:

- Turn it into a real portfolio project later.

Data Engineering additions:

- Track quiz attempts as events.
- Model user attempts, questions, topics, scores, weak topics.
- Create analytical tables.
- Add dashboard or metrics page.
- Add seed data.
- Add CI.
- Add README and HANDOFF.

## Application Readiness Checklist

Start applying when:

- LinkedIn is updated.
- Resume EN is improved.
- Portfolio is public and not embarrassing.
- At least one active project has a strong README.
- You can explain your current job in English for 2 minutes.
- You can explain one project in English for 3 minutes.
- You can answer "Why are you looking for remote roles?" clearly.

Suggested answer:

"I am currently in a hybrid role, but I am focusing my career on full remote data engineering opportunities. I work well with documentation, async communication, and structured delivery, and I am building my portfolio around practices that are common in remote teams, such as GitHub workflows, pull requests, CI/CD, and clear technical handoffs."
