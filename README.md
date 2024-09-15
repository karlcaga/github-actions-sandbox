We want the `pr` pipeline to run on PRs.

We want `cicd.yml` pipeline to run on pushes to main or on new semver tags.

Tagged commits that look like a semantic version number should also trigger the `cicd` the `build` job.
If the `build` job succeeds, then the `push_to_production` job should run.