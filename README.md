# dab-template

A Template for a Databricks Declarative Automation Bundle (DAB) project.

## Repository Structure

```text
forecasting-model-dab/
├── src/
│   └── forecasting_model/
│       ├── notebooks/
│       ├── jobs/
│       ├── pipelines/
│       ├── models/
│       └── utils/
├── tests/
│   ├── unit/
│   └── integration/
├── resources/
│   ├── jobs.yml
│   ├── pipelines.yml
│   └── clusters.yml
├── .github/
│   └── workflows/
│       ├── ci.yml
│       └── release.yml
├── .vscode/
│   ├── settings.json
│   └── extensions.json
├── databricks.yml
├── pyproject.toml
├── .pre-commit-config.yaml
├── requirements.txt
├── .gitignore
├── CHANGELOG.md
└── README.md
```

## Quickstart

```bash
databricks auth login --host <put the https link to your host here>
databricks bundle validate  
databricks bundle deploy
databricks bundle run hello_world_job
```
