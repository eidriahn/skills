---
name: pr-comment
description: Write and post comments on the user's pull requests. Use when the user wants to comment on a PR, reply to a review thread, or answer review feedback.
---

# PR comments

Every comment is **terse**: it states the outcome (what changed, and that it is done) in the fewest words that carry the full meaning. The reader is a reviewer who already knows the PR and can see the code.

## Steps

1. **Gather.** Read the PR and the thing being answered: `gh pr view`, `gh pr diff`, and the review threads (`gh api repos/{owner}/{repo}/pulls/{number}/comments`). Done when you can state every change the comment covers as one outcome each.
2. **Draft** the comment by the style below.
3. **Show** the draft to the user and post it only once they approve. A **long** draft (see below) is shown with a note that it runs long and why, and the user decides whether it goes out long or gets cut. A top-level comment goes through `gh pr comment <number> --body`. A reply goes into its review thread: `gh api repos/{owner}/{repo}/pulls/{number}/comments/{comment_id}/replies -f body=...`.

## Style

- **Outcome first**, past tense, one line per change: "Moved validation into the parser." "Renamed `fetchUser` to `getUser`."
- **One to three lines.** A reply to a single review thread is usually one: "Done, `retry` now backs off exponentially."
- **Long when the meaning needs it.** When a point cannot be stated in three lines without losing meaning (a trade-off, a disagreement, a design explanation), write it out in full, still with every sentence earning its place, and mark the draft **long** for the user's approval.
- **The change is the subject.** Describe what the code now does. The reviewer reads the code, not the history, so never mention commits: no SHAs, no commit links, no "Fixed in `ac6ac19`". Write "Moved the check into `parse()`.", not "Fixed in `ac6ac19`, moved the check into `parse()`."
- **Why only when it diverges**: add a short reason when the change differs from what the reviewer asked for, or when you chose not to change something.
- Wrap identifiers, files and commands in backticks.
