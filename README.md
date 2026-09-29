# cycle

Research-project lifecycle toolkit for Claude Code: a five-phase cycle closed by gates, two
decision gates (is the work worth writing up, is it worth disseminating), a five-artefact project
memory, a research-leads registry, a lab notebook, a consolidated state of knowledge, adversarial
pre-flight and post-result checks, scope triage, model and effort routing under usage quotas,
dataset versioning, project scaffolding, and a reboot procedure for resuming an interrupted
project. It accompanies the article series on the AI-augmented research environment of the
Guyeux group (FEMTO-ST).

This is a filtered release of the `cycle` plugin only. It is built from a fixed git state by
an export script kept with the article repository, which removes backup files and evaluation outputs, neutralises settings that
encode one author's habits (number of accounts, evening cut-off), and checks the result against an
exclusion list. Nothing else from the author's marketplace is included.

Portability. The skills were designed in the author's environment and keep its conventions as
defaults: projects under `~/docs/codes/`, a shared knowledge base under `~/.agents/knowledge/`,
and the optional coordination tooling of concurrently running sessions (not included). The
scaffolding root is set with `INIT_PROJECT_CODES_ROOT` and the project shortcut root with
`CYCLE_PROJECT_SHORTCUT_ROOT`. Number of accounts and evening cut-off of the usage-quota signal
are set with `CLAUDE_COMPTES_MAX` (default 1) and `CLAUDE_CUTOFF_HEURE` (default 24, no
deduction). References to files of the author's knowledge base are optional and degrade with an
explicit message when the file is absent. `narratif/scripts/plan_vs_manuscrit.py` reuses the
metrics scripts of a separate `deai-latex` skill, which is not part of this release, and says so
when they are missing.

Skill texts are mostly in French, the language of the author's projects.

License: MIT (see `LICENSE`). Citation: see `CITATION.cff`.
