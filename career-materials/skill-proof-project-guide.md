# Skill Proof and Portfolio Project Guide - Gabriel Franco

Goal: for every important skill in Gabriel's Data Engineering profile, define how to prove it publicly through certification, GitHub projects, LinkedIn material, or interview stories.

This file is sanitized for public portfolio use. It must not include internal system names, private company links, manager names, or real banking implementation details.

## Summary

| Skill | Proof | Project | Priority |
|---|---|---|---|
| SQL / Spark SQL | Databricks Associate, DP-750, HackerRank SQL | Config-driven SQL pipeline | High |
| Python | Public code with tests, typing, docs | Python ETL with BCB data | High |
| PySpark | Databricks Associate + notebooks | Financial PySpark transforms | High |
| Databricks / Delta Lake | Databricks Associate + DP-750 | Lakehouse financial data | Highest |
| Control-M | CV and interview story only | Batch concepts mapped to Airflow | Medium |
| Airflow | Astronomer certification + DAG repo | Airflow financial pipeline | High |
| Git / GitHub Actions | CI workflows + GitHub certification path | Data validation CI/CD | High |
| Power BI | Screenshots + `.pbix`, PL-300 optional | Financial dashboard | Optional |
| Documentation | Strong READMEs and handoffs | Every repo | Highest |

## Recommended Project Order

1. Lakehouse Financial Data
2. Python ETL + Tests + CI/CD
3. Config-Driven SQL Pipeline
4. Airflow Financial Pipeline
5. Power BI Financial Dashboard
6. Metadata-driven Financial Pipeline Lab
7. Spark Schema Validation Lab
8. Financial Enrichment Pipeline Lab

## Project 1 - Lakehouse Financial Data

Repo name: `lakehouse-financial-data`

Purpose: central portfolio project proving Databricks, Delta Lake, PySpark, SQL, medallion architecture, and financial-data thinking.

Scope:

- Public financial dataset, preferably BCB indicators or another non-confidential source.
- Bronze layer for raw data.
- Silver layer for cleaned and standardized data.
- Gold layer for analytics-ready indicators.
- Delta features such as MERGE, schema evolution, time travel, and table history.
- Notebook exported from Databricks as `.py` or `.ipynb`.
- README with architecture diagram, commands, assumptions, and lessons learned.
- `HANDOFF.md` for continuation.

## Project 2 - Python ETL + Tests + CI/CD

Repo name: `python-etl-bcb`

Purpose: prove Python engineering quality, not just scripting.

Scope:

- Read public BCB API or CSV data.
- Clean, normalize, aggregate, and save output.
- Use tests with `pytest`.
- Add lint with `ruff`.
- Add GitHub Actions workflow.
- Add a CI badge to the README.
- Document schema and failure handling.

## Project 3 - Config-Driven SQL Pipeline

Repo name: `config-driven-sql-pipeline`

Purpose: publicly demonstrate the same reasoning behind financial rule parameterization, with fictional data and rules.

Scope:

- Input rules in CSV or YAML.
- Python reads the configuration and generates SQL.
- SQL runs in DuckDB or SQLite.
- Output table stores calculated results.
- Tests validate schema and sample outputs.
- README explains config-driven/metadata-driven design.

## Project 4 - Airflow Financial Pipeline

Repo name: `airflow-financial-pipeline`

Purpose: bridge the Control-M experience into modern Apache Airflow orchestration proof.

Scope:

- Docker Compose Airflow setup.
- DAG with:
  - FileSensor for input file arrival.
  - Ingestion task.
  - Transformation task.
  - Validation task.
  - Success marker task.
- Retries, timeout, logs, and failure callback.
- Optional XCom metadata passing.
- README explaining the translation from Control-M batch orchestration concepts to Airflow patterns.

## Project 5 - Power BI Financial Dashboard

Repo name: `powerbi-financial-dashboard`

Purpose: keep Power BI visible as a secondary skill and connect analytics background to Data Engineering.

Scope:

- BCB indicators such as Selic, IPCA, and exchange rates.
- Power Query transformations.
- DAX measures such as moving average and percentage variation.
- Screenshots and `.pbix`.
- README explaining data source and metrics.

## Project 6 - Metadata-driven Financial Pipeline Lab

Repo name: `metadata-driven-financial-pipeline`

Purpose: demonstrate how complex financial transformations can be controlled by metadata instead of hardcoded logic.

Scope:

- Synthetic input metadata defining sources, fields, joins, filters, and output columns.
- Spark SQL or DuckDB implementation that builds a query from metadata.
- Fake financial datasets only.
- Validation that compares expected output schema and generated query behavior.
- README explaining metadata-driven design and limitations.

## Project 7 - Spark Schema Validation Lab

Repo name: `spark-schema-validation-lab`

Purpose: demonstrate schema validation, data type checks, and debugging of Spark write issues in a safe public scenario.

Scope:

- Synthetic DataFrames and target schemas.
- Examples of column order mismatch, type mismatch, null handling, and target table compatibility.
- Tests that catch schema drift before writing.
- README explaining why schema validation matters in production pipelines.

## Project 8 - Financial Enrichment Pipeline Lab

Repo name: `financial-enrichment-pipeline`

Purpose: show a sanitized version of modernizing a legacy financial rule into an enrichment layer with traceability and parity checks.

Scope:

- Synthetic fixed-income-like data.
- Legacy calculation represented as a simple SQL rule.
- New enrichment table with keys, calculation fields, source traceability, and validation columns.
- Parity report comparing legacy output and new enrichment output.
- README with before/after architecture.

## Certification Order

Immediate sprint:

1. Databricks Certified Data Engineer Associate.

After the immediate sprint:

1. AZ-900.
2. DP-750.
3. GitHub Actions / CI-CD path.
4. Astronomer Certification for Apache Airflow Fundamentals.
5. GitHub Foundations if quick and useful.
6. PL-300 only if Gabriel wants to keep Power BI as a stronger secondary track.

## Public Source Ideas

- Banco Central do Brasil Open Data: `https://dadosabertos.bcb.gov.br/`
- BCB SGS time series API: `https://api.bcb.gov.br/dados/serie/bcdata.sgs.{codigo}/dados`
- Databricks Community Edition: `https://community.cloud.databricks.com/`
- HackerRank SQL: `https://www.hackerrank.com/domains/sql`
- Astronomer Academy: `https://academy.astronomer.io/`
- GitHub Foundations: `https://education.github.com/experiences/foundations_certificate`

## Evidence Standard

Every portfolio repo should include:

- `README.md`
- `HANDOFF.md`
- Clear folder structure.
- Setup/run instructions.
- Architecture diagram or Mermaid flow.
- Tests when applicable.
- GitHub Actions when applicable.
- No real company data, secrets, private links, or internal system names.
