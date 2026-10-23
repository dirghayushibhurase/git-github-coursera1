# Final Project Submission Answers
# GitHub UI and Git CLI — Introduction to Git and GitHub
# Student: dirghayushibhurase
# Date: 2026-10-23

---

## Part A — Public GitHub File URLs (Tasks 1–5)

| Task | File | Public URL | Status |
|------|------|-----------|--------|
| 1 | README.md | https://github.com/dirghayushibhurase/git-github-coursera1/blob/main/README.md | ✅ PASS |
| 2 | LICENSE | https://github.com/dirghayushibhurase/git-github-coursera1/blob/main/LICENSE | ✅ PASS |
| 3 | CODE_OF_CONDUCT.md | https://github.com/dirghayushibhurase/git-github-coursera1/blob/main/CODE_OF_CONDUCT.md | ✅ PASS |
| 4 | CONTRIBUTING.md | https://github.com/dirghayushibhurase/git-github-coursera1/blob/main/CONTRIBUTING.md | ✅ PASS |
| 5 | simple-interest.sh | https://github.com/dirghayushibhurase/git-github-coursera1/blob/main/simple-interest.sh | ✅ PASS |

---

## Part B — File Verification Details

### Task 1: README.md
- Content: "# Introduction to Git and GitHub" / "Simple Interest Calculator" section
- URL: https://github.com/dirghayushibhurase/git-github-coursera1/blob/main/README.md
- Status: ✅ Present and correct

### Task 2: LICENSE
- Type: Apache License Version 2.0
- Copyright: 2020 IBM Developer Skills Network
- Size: 202 lines / 11,358 bytes
- All required sections present: Definitions, Terms and Conditions (sections 1–9), Appendix
- URL: https://github.com/dirghayushibhurase/git-github-coursera1/blob/main/LICENSE
- Status: ✅ Complete Apache 2.0 license

### Task 3: CODE_OF_CONDUCT.md
- Sections present:
  - ✅ Our Pledge
  - ✅ Our Standards
  - ✅ Enforcement Responsibilities
  - ✅ Scope
  - ✅ Enforcement
  - ✅ Enforcement Guidelines (Correction, Warning, Temporary Ban, Permanent Ban)
  - ✅ Attribution (Contributor Covenant v2.0)
- URL: https://github.com/dirghayushibhurase/git-github-coursera1/blob/main/CODE_OF_CONDUCT.md
- Status: ✅ All required sections present

### Task 4: CONTRIBUTING.md
- Required sentence present: "All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome."
- URL: https://github.com/dirghayushibhurase/git-github-coursera1/blob/main/CONTRIBUTING.md
- Status: ✅ Exact required sentence present

### Task 5: simple-interest.sh
- Prompts for: principal (p), rate of interest per year (r), time period in years (t)
- Calculation: s=$(expr $p \* $t \* $r / 100)
- Outputs: "The simple interest is: " followed by value
- URL: https://github.com/dirghayushibhurase/git-github-coursera1/blob/main/simple-interest.sh
- Status: ✅ Correct

---

## Part C — CLI Evidence Files (Tasks 6–9)

### Task 6: forked-repo
- Evidence file: https://github.com/dirghayushibhurase/git-github-coursera1/blob/main/forked-repo
- Command: gh api repos/dirghayushibhurase/git-github-coursera1 --jq '{name:.name, fork:.fork, parent:.parent}'
- Actual result: { "fork": false, "parent": null }
- ⚠️ INCOMPLETE: Repository was NOT created via GitHub's Fork button.
  GitHub API reports fork:false. The upstream IBM repo is configured only as
  a local git remote, not as the GitHub parent. See ACTION REQUIRED below.

### Task 7: merge_branches
- Evidence file: https://github.com/dirghayushibhurase/git-github-coursera1/blob/main/merge_branches
- Branch: bug-fix-typo (created from main, pushed to origin)
- Typo fixed: "Addtional Authors" -> "Additional Authors" in simple-interest.sh
- Merge result: Fast-forward, 1 file changed, 1 insertion(+), 1 deletion(-)
- Commits: b65c078..e9a4bb6
- Status: ✅ COMPLETE — real merge output captured

### Task 8: bug-fix-revert
- Evidence file: https://github.com/dirghayushibhurase/git-github-coursera1/blob/main/bug-fix-revert
- Pull Request URL: https://github.com/dirghayushibhurase/git-github-coursera1/pull/1
- PR Number: 1
- PR State: open
- Head branch: bug-fix-revert (dirghayushibhurase/git-github-coursera1)
- Base branch: main (dirghayushibhurase/git-github-coursera1)
- Created: 2026-10-23T18:39:10Z
- Status: ✅ COMPLETE — real PR created and API response captured

### Task 9: github-branches
- Evidence file: https://github.com/dirghayushibhurase/git-github-coursera1/blob/main/github-branches
- Local branches: main, bug-fix-typo, bug-fix-revert
- Active branch: main
- Remote branches (origin): main, bug-fix-typo, bug-fix-revert
- Remote branches (upstream): main
- git status: On branch main, up to date with origin/main, nothing to commit, working tree clean
- Status: ✅ COMPLETE — real branch listing captured

---

## ⚠ ACTION REQUIRED FROM YOU (Task 6 — Fork Status)

The repository `dirghayushibhurase/git-github-coursera1` was created as a new
repo (not forked). The GitHub API returns `"fork": false` and `"parent": null`.

To fix this, you need to:

1. Go to: https://github.com/ibm-developer-skills-network/mcino-Introduction-to-Git-and-GitHub
2. Click the **Fork** button (top-right)
3. In "Owner", select **dirghayushibhurase**
4. In "Repository name", type: **git-github-coursera1** (or another name)
5. Click **Create fork**

OR — if the assignment accepts the upstream remote configuration as evidence,
the `forked-repo` file already contains the local git remote proof.

Once forked properly, the curl command will return:
  "fork": true,
  "parent": { "full_name": "ibm-developer-skills-network/mcino-Introduction-to-Git-and-GitHub" }

---

## Repository Summary

| Item | Value |
|------|-------|
| Fork URL | https://github.com/dirghayushibhurase/git-github-coursera1 |
| Upstream URL | https://github.com/ibm-developer-skills-network/mcino-Introduction-to-Git-and-GitHub |
| Active branch | main |
| All branches | main, bug-fix-typo, bug-fix-revert |
| Open PRs | PR #1 (bug-fix-revert → main) |
| GitHub CLI | gh v2.103.0, authenticated as dirghayushibhurase |
