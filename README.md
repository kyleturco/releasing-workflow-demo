# Release Workflow - Demo/Presentation

## Releasing
- Create a pull request from `staging` -> `master`. This PR should be titled with "Release" and the date e.g., ("Release 06_06_2018")
- Checkout `master` locally, ensure it's up to date with the remote master.
- Run `git merge staging` to perform a fast-forward merge -- do not create a merge commit.
- Important: Start the project locally to confirm everything still looks correct.
- Tag the commit with `git tag {your version}` - e.g., `git tag v1.1.0`
- Push the updated branch and the new tag to remote: `git push origin master --tags`
- Go to the releases tab in the project, find your latest tag, hit edit, and add some docs about what's in that release. If proper commit organization has been used, this can be as easy as listing all the commits that were in `staging`
