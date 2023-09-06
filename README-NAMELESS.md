# Add the upstream repo as a remote
git remote add upstream git@github.com:blockscout/frontend.git

# Fetch the latest commits
git fetch upstream

# Switch to local master branch
git checkout main

# Replay our master branch changes over the upstream master branch
git rebase upstream/main

git push --force