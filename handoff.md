# Handoff Notes

## Snapshot
- Date: 2026-03-02
- Workspace: `/Users/tmasingale/Documents/GitHub/github-starter-tutorial`
- GitHub owner: `sicxz`

## What Was Completed

### 1) Two assignment repos were created and published
- Week 8 repo: <https://github.com/sicxz/wk8-link-dashboard-assignment>
- Project #5 repo: <https://github.com/sicxz/project5-research-dashboard-assignment>

### 2) README specs were added in both repos
- Week 8 README: <https://github.com/sicxz/wk8-link-dashboard-assignment/blob/main/README.md>
- Project #5 README: <https://github.com/sicxz/project5-research-dashboard-assignment/blob/main/README.md>

### 3) Labels were created in both repos
- `step`, `setup`, `antigravity`, `design`, `feature`, `git`, `deploy`, `submission`, `resources`

### 4) Milestones were created
- **Week 8 repo**
  - `Foundation`
  - `Build and Iterate`
  - `Deploy and Submit`
- **Project #5 repo**
  - `Planning and Build`
  - `Design and Upgrades`
  - `Deploy and Submission`

### 5) Full issue sets were created (8 each)
- Week 8 issues: <https://github.com/sicxz/wk8-link-dashboard-assignment/issues>
- Project #5 issues: <https://github.com/sicxz/project5-research-dashboard-assignment/issues>

### 6) Issue templates were added in both repos
- `.github/ISSUE_TEMPLATE/step.md`

### 7) Original onboarding repo was linked to both assignment repos
- Updated file: `/Users/tmasingale/Documents/GitHub/github-starter-tutorial/README.md`
- Commit already pushed.

## Current Blocker
Project boards could not be created because the GitHub CLI token is missing scopes:
- `project`
- `read:project`

Error seen:
- `your authentication token is missing required scopes [project read:project]`

## Resume Steps on Other Computer

### 1) Clone/pull repos
- `github-starter-tutorial`
- `wk8-link-dashboard-assignment`
- `project5-research-dashboard-assignment`

### 2) Re-auth GitHub CLI with project scopes
```bash
gh auth refresh -h github.com -s project,read:project
```

### 3) Verify auth
```bash
gh auth status -h github.com
gh project list --owner sicxz
```

### 4) Create project boards (one per assignment)
Suggested names:
- `WK8 Assignment Progress`
- `Project 5 Assignment Progress`

Then add custom fields/status columns:
- `To Do`
- `In Progress`
- `Done`

Then add all open issues from each repo to the matching board in `To Do`.

## Quick Verification Commands
```bash
gh issue list --repo sicxz/wk8-link-dashboard-assignment --state open --limit 20
gh issue list --repo sicxz/project5-research-dashboard-assignment --state open --limit 20
gh repo view sicxz/wk8-link-dashboard-assignment --json url,defaultBranchRef,description
gh repo view sicxz/project5-research-dashboard-assignment --json url,defaultBranchRef,description
```

## Repo State Notes
- `wk8-link-dashboard-assignment`: clean, synced to `origin/main`
- `project5-research-dashboard-assignment`: clean, synced to `origin/main`
- `github-starter-tutorial`: includes this handoff file and previously pushed README links to both assignment repos

## Optional Next Improvements
1. Add screenshot assets for issue bodies.
2. Add GitHub Project board automation script for repeatable setup.
3. Add assignment rubrics with finalized point values in each README.
