# GAEE Ω-∞

GAEE is a lightweight control-plane foundation for secure, fault-tolerant orchestration with trusted execution environment readiness signals.

## Included

- FastAPI backend exposed on port 8000
- backend engine with GAEE state constants
- static control-plane frontend for GitHub Pages
- deployment workflow for GitHub Pages
- pytest suite with 3 passing checks

## Run locally

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
uvicorn api.main:app --host 0.0.0.0 --port 8000
```

## Test

```bash
pytest -q
```

## Deployment

The repository includes a GitHub Pages deployment workflow for `frontend/control_plane`.
