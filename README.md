# org-structure
This repo is made to track a number of restructings that is about to take place soon, and also to keep track of the new structure.

Here are some TODOs:
1. Rename repos to follow a standard.
2. Document to track old names versus new names. Done, see - [track-repo-rename](track-repo-rename.md)
3. Create github projects and link to repos (note: Some projects have two repos - backend(server), frontend(client))
4. Add contributing.md file to all repos, add code of conduct.
5. Implement workflows to move issues and pull requests around in the github project, so the github project is fully automated.
6. Review role permissions in github org.
7. Add repo to teach interns how to use github.
8. Setup ci/cd for all repos.
9. Update the website urls to the production urls for each repo not the vercel dev deployment urls currently there.

Changing the org name from `unibeninterns` to `drid-uniben` already broke stuff for repos whos deployment mode is that changes get pulled into a vps, in that case to fix, first run:
``bash
git remote -v
```
to confirm that it is using the old name uniben interns, if true, you wan update the url like this:
```bash
# This assumes git remote -v showed origin as your remote
git remote set-url origin ${basically the same url you saw when you ran git remote -v, just only change the org name from unibeninterns to drid-uniben}
```
