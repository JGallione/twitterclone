# Shared Claude Code sessions

This folder holds Claude Code session transcripts for this project, shared with gitclaudehub.

- `index.json` lists the sessions.
- `sessions/<id>.jsonl` is each transcript. Project paths are stored as `{{GITCLAUDEHUB_ROOT}}`
  and likely secrets are replaced with `[REDACTED]` before they are committed.

To continue a session in your own terminal, install the `gitclaudehub` command
(`npm install -g github:JGallione/gitclaudehub`, needs Node 18.17+ and git), then:

```bash
gitclaudehub pull              # installs the shared sessions for this checkout
claude --resume <id>
gitclaudehub push <id>         # shares your new turns (and code) back
```
