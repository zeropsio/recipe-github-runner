- Import a service:
```yaml
services:
  - hostname: myrunner
    buildFromGit: https://github.com/zeropsio/recipe-github-runner
    envSecrets:
      GITHUB_RUNNER_TOKEN: xxx
      RUNNER_REPO: https://github.com/foo/bar
```
- Fill in token from `https://github.com/[my-org]/[my-repo]/settings/actions/runners/new` and repository.
- Runner will automatically register.
