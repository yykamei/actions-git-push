# actions-git-push

This is a composite GitHub Actions for my projects; it's responsible for running git-push(1).

```yaml
name: Changelog
on: [push, pull_request]
jobs:
  changelog:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - run: DO SOMETHING
      - uses: yykamei/actions-git-push@main
        with:
          commit-message: DO SOMETHING
          branch: MY-SPECIAL-BRANCH
```
