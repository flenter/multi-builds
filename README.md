Shows how to trigger a build with a different yaml from wercker.

It achieves this by removing the git history, update the wercker.yml and
doing a push on to a `$BRANCH_NAME-integration` branch

### HOWTO

To use this, you need to add a pipeline variable:

`GIT_REMOTE` with a valid personal access token. Create your token here:
https://github.com/settings/applications#personal-access-tokens

The value for git remote should be something like the following:

https://{{username}}:{{token}}@github.com/{{owner}}/{{repo_name}}.git
