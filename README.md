# .github (org defaults)

**Public** repository (no sensitive content). GitHub only applies org-wide issue/PR templates from a public
`.github` repo; workflow templates here are offered in every repo's Actions → New workflow page.

| Path | Purpose |
|---|---|
| `workflow-templates/*.yml` + `*.properties.json` | starter callers of `platform-workflows@v1` |
| `PULL_REQUEST_TEMPLATE.md`, `ISSUE_TEMPLATE/` | org defaults (a repo's own template wins) |
| `profile/README.md` | public org profile (member-only profile lives in `.github-private/profile/`) |

If your enterprise uses Enterprise Managed Users (no public repos), make this repo internal: workflow
templates still work for internal/private repos, but PR/issue templates must then ship per repo (app-template already does).
