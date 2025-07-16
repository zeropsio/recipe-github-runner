- Create your own repo from this template
- Fill in token from `https://github.com/[my-org]/[my-repo]/settings/actions/runners/new` and repository.
- Change [zerops.yml](https://github.com/zeropsio/recipe-github-runner/blob/main/zerops.yml#L4) to select runner primary technology through `run.base` or install any additional dependencies in `run.prepareCommands`

- Import a service:
```yaml
services:
  - hostname: myrunner
    buildFromGit: https://github.com/[my-org]/recipe-github-runner
    envSecrets:
      GITHUB_RUNNER_TOKEN: xxx
      RUNNER_REPO: https://github.com/foo/bar
```


Runner will automatically register.
