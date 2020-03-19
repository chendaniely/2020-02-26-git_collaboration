# 2020-02-26 Git training for collaboration

- `clone`: "downloading" a repository from a remote to our local computer
  - You only really need to do this once, just like the `init` command
- `branch <name>`: create a branch called <name>
  - `checkout <name>` or `switch <name>`: to move `HEAD` (i.e., switch) to that branch
  - `push <branch>` `pull <branch>`: we need to be more mindful which branch we want to push/pull, and not automaticall type `master`
  - `checkout -b <name>`: this will create and checkout the branch in one command

- Pull request (aka merge request): this is how you `merge` branches on the web interfance (e.g., GitHub, BitBucket)
  - This is also where you choose which branch you are going to merge into (default `master`)
  - In here there is a conversation and "files change" tab, this is where you do code review
  - When you're ready, click the greeen "merge pull request" button
  - don't forget to delete your branch

## Update our local computer

- Make sure you are on the master branch
- update your system with `git pull origin master`
- `fetch --prune --all`: to clean up all your references on all your remotes
- `branch -d <branch>`: will delete a branch

- `merge <branch>`: incorporates `<branch>` into your current branch

- `rebase` and `cherry-pick`: are ways to re-write history or incorate other commits into current history

- There are different collaboration workflows
  - https://www.atlassian.com/git/tutorials/comparing-workflows
  - direct collaborator
  - branching
  - forking 
