# merge-queue-test-2
## Scenario 3, second PR

Queued behind branch-2. Branched from main before branch-2 merged,
so its queue branch base should contain branch-2 commit.

## Scenario 4, good PR

Queued behind the failing PR. Should still merge after that one is
ejected, rebuilt on a base that does not contain it.

## Scenario 10, first merge

Changes README.md only. Nothing under dbt/, so the PR queued behind
this one should still report SKIP.
