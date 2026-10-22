# heroverse-runner

Execution runner only. Its single workflow checks out the public HeroVerse
engine with a fine-grained token and runs the engine's own render script
(`migration/ci/render_pilot.sh`); results are written back to the engine
repository. No code, scripts, media or credentials live here.

Only the repository owner can start the workflow; secrets are never exposed to
forks or pull requests.

This repository is still the live renderer, not an obsolete duplicate. The
authoritative workflow is `.github/workflows/render.yml`; the old copy in the
engine was archived on 2026-10-22. The token remains necessary for authorized
writes to the engine. Repository visibility does not authorize credential exposure.
`PUBLIC_LOGS=1` limits console output; it does not make release attachments private.
