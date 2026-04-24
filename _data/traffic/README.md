# Traffic Data

This directory stores automated traffic analytics collected by GitHub Actions.

## Setup

1. **Create a fine-grained Personal Access Token (PAT):**
   - Go to [github.com/settings/tokens](https://github.com/settings/tokens?type=beta)
   - Create a token scoped to `github-education-resources/teacher-toolbox`
   - Grant **Administration: Read** permission (required for traffic API)
   - Grant **Contents: Read and write** permission (required to commit data)

2. **Add the token as a repository secret:**
   - Go to the repo → Settings → Secrets and variables → Actions
   - Create a secret named `TRAFFIC_TOKEN` with the PAT value

3. **Create the `traffic-report` label** (optional):
   - Go to Issues → Labels → New Label
   - Name: `traffic-report`, Color: `#0075ca`

## How It Works

| Workflow | Schedule | What it does |
|----------|----------|--------------|
| `collect-traffic.yml` | Daily at 06:00 UTC | Fetches views, clones, top pages & referrers; saves normalized daily JSON files |
| `monthly-report.yml` | 2nd of each month at 08:00 UTC | Aggregates the previous month's data into a Markdown report and GitHub Issue |

Both workflows can also be triggered manually via `workflow_dispatch`.

## Data Structure

```
_data/traffic/
├── daily/
│   ├── 2026-04-10.json    # One file per UTC day
│   ├── 2026-04-11.json
│   └── ...
├── reports/
│   ├── 2026-04.md         # Monthly Markdown report
│   └── ...
└── README.md              # This file
```

Each daily JSON file contains:

```json
{
  "date": "2026-04-10",
  "views": { "count": 74, "uniques": 46 },
  "clones": { "count": 3, "uniques": 3 },
  "paths_snapshot": [ ... ],
  "referrers_snapshot": [ ... ]
}
```

## Important Notes

- **Views/clones** are precise per-day metrics from the GitHub Traffic API.
- **Paths and referrers** are rolling 14-day snapshots (GitHub does not provide daily breakdowns). Monthly reports rank these by how often a page appeared in the daily top-10, not by exact monthly totals.
- The daily collector **rewrites the last 14 days** on each run to capture corrections from the API. This is by design — it ensures accuracy.
- If collection is missed for >14 consecutive days, that data is **permanently lost**. The workflow includes gap detection warnings.
