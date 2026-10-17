# heroverse-runner

Execution runner only. Its single workflow checks out the private HeroVerse
engine with a fine-grained token and runs the engine's own render script
(`migration/ci/render_pilot.sh`); results are written back to the private
repository. No code, scripts, media or credentials live here.

Only the repository owner can start the workflow; secrets are never exposed to
forks or pull requests.

**Status: disabled (2026-10-17).** GitHub's terms for Actions do not allow a repository's runners to be
used for work unrelated to that repository's own software project. Renders run in the private engine's
own workflows instead. No secrets are needed here.
