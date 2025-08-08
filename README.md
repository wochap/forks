# forks

A repository for managing my forks more easily. It provides commands to rebase against upstream fork branches.

## Gettings started

```sh
# run once
$ just init

# flow to update forks
$ just check-upstream
$ just rebase-all
# $ just rebase {{repository_folder_name}}

```

## Adding new forks

```sh
$ git submodule add git@github.com:wochap/dircolors.git
# then update init in Justfile
```

## TODOs:

- [ ] delete zsh-autocomplete
- [ ] delete slurp

