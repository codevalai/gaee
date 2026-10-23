# GAEE Ω-∞

GAEE is a production-oriented control-plane foundation for resilient orchestration, secure runtime monitoring, and TEE-aware governance.

## Highlights

- FastAPI API with health and status endpoints
- fault-tolerant runtime state monitoring
- GitHub Pages-ready control-plane front end
- CI workflow with pytest validation
- release checklist for shipping and deployment

## Local development

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
uvicorn api.main:app --host 0.0.0.0 --port 8000
```

## API

- `GET /` returns the GAEE status payload
- `GET /health` returns a simple health-check response

## Test suite

```bash
pytest -q
```

Expected result:

```text
3 passed
```

## Deploy to GitHub Pages

The repository includes a Pages workflow at `.github/workflows/deploy-gaee-control-plane.yml` which publishes `frontend/control_plane`.

## Release checklist

See `RELEASE_CHECKLIST.md` for the complete publish and validation flow.
