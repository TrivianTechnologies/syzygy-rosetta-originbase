# Fork Detachment Provenance Record

**Repository:** `TrivianTechnologies/syzygy-rosetta-originbase`  
**Recorded:** 2026-10-01  
**Purpose:** Preserve repository-network provenance before converting this public fork into a standalone historical repository.

## Status before detachment

- GitHub fork: **yes**
- Upstream: `liangmeili686/rosetta-rewrite`
- Visibility: public
- Default branch: `main`
- Intended role after detachment: **historical provenance / origin codebase**
- GitHub UI reported `main` as **12 commits ahead** of upstream `main` during preparation.
- Releases observed: none
- Child forks observed: none

## Preserved branches

| Branch | Head SHA |
|---|---|
| `main` | `ef91eaf0433c23b990f09325ea8bdc4dacf72413` |
| `repo-hardening-cleanup` | `eb4487a97335de5239914cb15aae79b22f02c4d0` |
| `evaluate-interaction-contract` | `4cd9fb61f9d304d3d67f340e061d091d561c44e6` |

## Pull request metadata preserved before detachment

GitHub warns that leaving a fork network does not retain issues, pull requests, wikis, stars, watchers, comments, child forks, or other fork-network metadata. The open pull request below is therefore recorded here before detachment.

### PR #1 — Add input-output interaction contract for evaluate

- Author: `FaiyazAzam`
- State at capture: open, unmerged
- Created: 2026-05-14T20:59:46Z
- Updated: 2026-05-15T16:46:05Z
- Base: `repo-hardening-cleanup`
- Base SHA: `eb4487a97335de5239914cb15aae79b22f02c4d0`
- Head: `evaluate-interaction-contract`
- Head SHA: `4cd9fb61f9d304d3d67f340e061d091d561c44e6`
- GitHub-recorded merge commit candidate: `ccb573a39339bd97fdfe7d9c2a2c76fa91668440`
- Test result reported in PR description: `54 passed`
- Comments observed: none

Summary recorded from the PR:

- adds optional `output` to the `/evaluate` request contract;
- evaluates both user/customer input and model output when output is provided;
- scores the input-output pair rather than comparing input to itself;
- applies safety, sensitive-topic, and policy checks to model output;
- adds output-prefixed violations such as `output:high_risk_content`;
- records `output` in evaluation audit logs;
- updates documentation, demo checklist, and example usage.

The branch itself remains part of Git history even though the GitHub pull-request object will not survive detachment.

## Detachment intent

This repository is being detached from its upstream fork network so its continued existence, governance, and historical record do not depend on the upstream account or repository.

Detachment does **not** rewrite authorship, contribution history, or Git commit metadata. Historical contributors remain attributable in the Git record.

This file records technical provenance. It does not attempt to restate contractual or legal terms.
