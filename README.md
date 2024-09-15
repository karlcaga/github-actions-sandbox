We want the `test_and_lint` pipeline to run on pushes to main and PRs.

We want `cicd.yml` pipeline to run after `test_and_lint` successfully runs.

Tagged commits that look like a semantic version number should also trigger the `cicd` the `build` job.
If the `build` job succeeds, then the `push_to_production` job should run.