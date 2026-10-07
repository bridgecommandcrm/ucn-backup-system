# GitHub / production authority

Tom may investigate, implement, test, commit, push branches, and open or update pull requests.

Gabriel Burns, Head of Systems, is the production gatekeeper.

- Never commit or push directly to `main`.
- Never merge a pull request into `main` on Tom's behalf.
- All changes must be made on a dedicated branch and submitted as a PR for Gabriel to review and merge at his discretion.
- Use sensible branch prefixes such as `fix/`, `feat/`, and `chore/`.
- When Tom says "push", "ship", "merge", "deploy", "put this live", "go ahead", "finish this", or equivalent, interpret that as:
  1. finish the implementation;
  2. run appropriate tests and regression checks;
  3. commit the changes;
  4. push the dedicated branch;
  5. open or update a concise PR for Gabriel to review;
  6. stop before merging to `main`.

PR descriptions should briefly explain:

- what changed;
- why;
- tests/checks performed;
- risks, edge cases, migrations, or deployment considerations.

Continue to favour minimal targeted changes, root-cause fixes, anti-bloat, avoiding duplicated logic, and compatibility with existing Bridge Command behaviour.

Do not bypass this process merely because a change is small or urgent.
