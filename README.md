# running-platform

A learning project: ingest running data from FIT files, build features, train a model,
serve it, and deploy it.

## Setup

```bash
make install    # uv sync + install pre-commit hooks
make lint       # ruff check + format check
make typecheck  # mypy (strict)
make test       # pytest
```

## Layout

```
src/running_platform/   ingest, features, training, serving
tests/
data/raw/               raw FIT files (gitignored)
data/processed/         derived datasets (gitignored)
models/                 trained artifacts (gitignored)
deploy/k8s/             Kubernetes manifests
```

## Build stages

- [ ] 1. FIT parser
- [ ] 2. Activity summaries
- [ ] 3. Daily features
- [ ] 4. First model
- [ ] 5. FastAPI service
- [ ] 6. Docker
- [ ] 7. Concurrency scripts
- [ ] 8. Kubernetes on kind
- [ ] 9. CI image build
