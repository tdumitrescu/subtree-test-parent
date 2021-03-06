Experimenting with `git subtree`. Links up https://github.com/tdumitrescu/subtree-test-child as a subtree in `lib/external`.

Steps taken to set up subtree initially:
- Add remote and fetch: `git remote add -f subtree-test-child git@github.com:tdumitrescu/subtree-test-child.git`
- Add commits (without squashing) and code from remote into `lib/external`: `git subtree add --prefix lib/external/subtree-test-child subtree-test-child master`

To push to subtree's separate repo:
- `git subtree push --prefix=lib/external/subtree-test-child/ subtree-test-child <branch>`

Pulling from subtree's remote:
- `git subtree pull --prefix=lib/external/subtree-test-child/ subtree-test-child <branch>`
