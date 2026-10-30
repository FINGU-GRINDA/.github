# .github

## 요약
FINGU-GRINDA 조직의 GitHub 프로필 페이지(github.com/FINGU-GRINDA)를 띄우는 레포다. 실제 내용은 `profile/README.md`(영문 회사 소개 + 한국어 요약: Rinda·Ara·TradeGraph·claude-rinda-plugin)와 배너 이미지 `profile/assets/banner.png` 뿐이며, 코드·공용 워크플로·org 기본 템플릿은 일부러 두지 않는다. 프로필 문구를 고칠 때는 `profile/` 만 수정한다. 2026-10-30 에 public 으로 바꾸고 Security gate 절차(ruleset 24047185 include, 20582782 exclude)를 마쳤다.

This repository only powers the public profile of [github.com/FINGU-GRINDA](https://github.com/FINGU-GRINDA). The page is `profile/README.md`; its images live in `profile/assets/`.

## Guardrail: edit `profile/` only

GitHub treats some files in an organization's `.github` repository as defaults for every repository in the org that lacks its own copy. Adding any of them here would change how all of our repositories behave, so they are intentionally absent:

`CONTRIBUTING.md` · `CODE_OF_CONDUCT.md` · `SECURITY.md` · `SUPPORT.md` · `GOVERNANCE.md` · `FUNDING.yml` · `ISSUE_TEMPLATE/` · `DISCUSSION_TEMPLATE/` · `PULL_REQUEST_TEMPLATE*` · `workflow-templates/`

If an org-wide default is ever needed, propose it in a separate PR and agree on it with the dev team first.

## Security gate

This repository is public, so it follows the public-repository procedure in the [security-gate-public](https://github.com/FINGU-GRINDA/security-gate-public) runbook: included in ruleset 24047185 and excluded from ruleset 20582782. Pull requests here cannot merge until both are in place.
