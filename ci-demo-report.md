# CI Demo Workshop Report

Live walkthrough of a change travelling through GitHub: feature branch → pull request → CI → merge.

## Account
- GitHub numeric user id: **28861483** (looked up by display name "Hezi Liu"; login: HeziLiu)

## Repository
- Repository: **ci-demo-workshop** (public, initialized with a README)
- Default branch: `main`
- Feature branch: `demo-ci-workflow`

## Pull Request
- PR number: **#1**
- Title: "Add demo CI workflow"
- Branches: `demo-ci-workflow` → `main`
- Commit on the branch: `e888599d7bd91839d5be1b31ab4182d68cfff8fe`

## CI Workflow Run
- Run id: **39626785795**
- Workflow: "Demo CI" (`.github/workflows/demo-ci.yml`), triggered by event: `pull_request`
- Run number / attempt: 1 / 1
- Conclusion: **success**
- URL: https://github.com/mcpmark-eval-liuhezi/ci-demo-workshop/actions/runs/39626785795

### Usage / billable timing (as reported by the Actions usage API)
- `run_duration_ms`: **7000** (7.0 s)
- `billable.UBUNTU.total_ms`: **0**
- `billable.UBUNTU.jobs`: **1**
- `billable.UBUNTU.job_runs[0]`: job_id `119313972979`, duration_ms `0`

### Jobs
| Job | Status | Conclusion | Started (UTC) | Completed (UTC) | Duration |
| --- | --- | --- | --- | --- | --- |
| `greet` (ubuntu-latest, job id 119313972979) | completed | success | 2026-10-21T15:33:40Z | 2026-10-21T15:33:43Z | ~3 s |

Steps in the job: "Set up job" → "Print greeting" (`echo "Hello from the CI demo workflow!"`) → "Complete job", all succeeded.

### Files changed by the PR
| File | Status | Changes |
| --- | --- | --- |
| `.github/workflows/demo-ci.yml` | added | +11 / -0 |

(1 file changed, 1 commit, +11 additions, 0 deletions)

## Outcome
- Merge method used: **regular merge commit** (merge method "merge", not squash or rebase).
- The PR **is merged**: PR #1 is closed with `merged: true`, merged at 2026-10-21T15:34:30Z.
- Merge commit SHA: **11bc9cbc4e71e450250146bfe804592015d47d0f**
