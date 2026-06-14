# 🚀 Saifa AI — CI/CD Template

GitHub Actions: unit tests · security scan · AI code review

## Workflows
| File | Trigger | What it does |
|------|---------|-------------|
| `unit-test.yml` | push/PR | Tests + coverage comment |
| `security.yml` | push/PR/weekly | Gitleaks + CodeQL + Trivy + summary |
| `ai-review.yml` | PR | Claude Opus review comment |

## Setup
Add to **Settings → Secrets → Actions**:
- `ANTHROPIC_API_KEY` — required for AI review

## Stack
Default: Node.js 20. Python sections are commented in each workflow.
