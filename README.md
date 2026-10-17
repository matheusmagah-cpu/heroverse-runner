# heroverse-runner

Execution runner only. Its single workflow checks out the private HeroVerse
engine with a fine-grained token and runs the engine's own render script
(`migration/ci/render_pilot.sh`); results are written back to the private
repository. No code, scripts, media or credentials live here.

Only the repository owner can start the workflow; secrets are never exposed to
forks or pull requests.
