# useful-linux-commands

# Git

```
git fetch --all; git branch -r | grep -v '->' | sed "s,\x1B[[0-9;]*[a-zA-Z],,g" | while read remote; do echo $remote | sed 's/origin///' | xargs -L1 git checkout; git reset --hard $remote; done
````
