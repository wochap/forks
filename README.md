# forks

A repository for managing my forks more easily. It provides commands to rebase against upstream fork branches.

## Gettings started

```sh
# run once or everytime you add a new fork
$ just init

# flow to update forks
$ just check-upstream
$ just rebase-all
# $ just rebase {{repository_folder_name}}

```

## Adding new forks

```sh
$ git submodule add git@github.com:wochap/dircolors.git
# update init fn in Justfile, and then run
$ just init
```

## Deleting forks

```sh
# removing dircolors fork
$ git submodule deinit -f -- dircolors
$ git rm -f dircolors
$ rm -rf .git/modules/dircolors
# $ git config -f .gitmodules --remove-section submodule.dircolors
# delete it from init block in Justfile
```
