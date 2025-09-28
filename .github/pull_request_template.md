<!--
PR Template Index
Because GitHub does not provide a native UI selector for multiple templates without query parameters, this index helps you choose the correct specialized template.

Usage:
1. Pick the appropriate template below.
2. Click its link to open a pre-filled PR creation page (replace REPO_OWNER and REPO_NAME if not already substituted by GitHub).
3. If you already opened a PR, you can copy/paste the content manually.

Note: Links rely on the `template=` query parameter which only works when creating a NEW pull request (not editing an existing one).
-->

# Pull Request Template Index
Select the template that best matches your change type.

| Change Type | Template Link | When To Use |
|-------------|---------------|-------------|
| Feature / Enhancement | [feature.md](../../blob/main/.github/PULL_REQUEST_TEMPLATE/feature.md?plain=1) | Adding new behavior, APIs, data structures |
| Bug Fix / Patch | [patch.md](../../blob/main/.github/PULL_REQUEST_TEMPLATE/patch.md?plain=1) | Correcting incorrect behavior |
| Refactor (No Behavior Change) | [refactor.md](../../blob/main/.github/PULL_REQUEST_TEMPLATE/refactor.md?plain=1) | Structural improvement only |
| Tests Only | [test.md](../../blob/main/.github/PULL_REQUEST_TEMPLATE/test.md?plain=1) | Adding or modifying tests |
| Documentation | [docs.md](../../blob/main/.github/PULL_REQUEST_TEMPLATE/docs.md?plain=1) | README, design docs, comments |
| Chore / Perf / Infra | [chore-perf.md](../../blob/main/.github/PULL_REQUEST_TEMPLATE/chore-perf.md?plain=1) | Tooling, build, performance tweaks |

---

## One-Click Create (replace ORG/REPO if forked)
These links open the compare page with a template preloaded. You still must set the correct base & compare branches.

> NOTE: GitHub only honors `template=` when starting creation from the compare page before the PR exists.

- Feature: `https://github.com/ORG/REPO/compare/main...your-branch?quick_pull=1&template=feature.md`
- Patch: `https://github.com/ORG/REPO/compare/main...your-branch?quick_pull=1&template=patch.md`
- Refactor: `https://github.com/ORG/REPO/compare/main...your-branch?quick_pull=1&template=refactor.md`
- Docs: `https://github.com/ORG/REPO/compare/main...your-branch?quick_pull=1&template=docs.md`
- Tests: `https://github.com/ORG/REPO/compare/main...your-branch?quick_pull=1&template=test.md`
- Chore/Perf: `https://github.com/ORG/REPO/compare/main...your-branch?quick_pull=1&template=chore-perf.md`

Replace `your-branch` with the branch you want to merge.

---

## FAQ
**Q: I already opened the PR; can I swap templates?**  
A: Manually copy the contents from the target template file and edit the PR description.

**Q: Why not keep a single giant template?**  
A: Focus improves quality; reviewers quickly see what matters for that change type.

**Q: What if my change spans multiple categories?**  
A: Use the dominant type (usually feature or patch) and add an "Additional Scope" subsection.

**Q: Do I still need semantic titles?**  
A: Yes; enforced by commit/PR lint workflow.

---

## Minimal Generic Section (If You Pasted Only This)
Fill at least:
- Summary:
- Rationale:
- Test Evidence:
- Risk / Rollback:
- Linked Issue(s):

---

Happy contributing!
