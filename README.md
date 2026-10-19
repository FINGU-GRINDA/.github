# .github

This repository only powers the public profile of [github.com/FINGU-GRINDA](https://github.com/FINGU-GRINDA). The page is `profile/README.md`; its images live in `profile/assets/`.

## Guardrail: edit `profile/` only

GitHub treats some files in an organization's `.github` repository as defaults for every repository in the org that lacks its own copy. Adding any of them here would change how all of our repositories behave, so they are intentionally absent:

`CONTRIBUTING.md` · `CODE_OF_CONDUCT.md` · `SECURITY.md` · `SUPPORT.md` · `GOVERNANCE.md` · `FUNDING.yml` · `ISSUE_TEMPLATE/` · `DISCUSSION_TEMPLATE/` · `PULL_REQUEST_TEMPLATE*` · `workflow-templates/`

If an org-wide default is ever needed, propose it in a separate PR and agree on it with the dev team first.

## Security gate

This repository is public, so it follows the public-repository procedure in the [security-gate-public](https://github.com/FINGU-GRINDA/security-gate-public) runbook: included in ruleset 24047185 and excluded from ruleset 20582782. Pull requests here cannot merge until both are in place.
