# Vendoring dependencies

This directory holds vendored dependencies, managed via [git subtrees](0).
All commands should be run from the top level of the repository.

[0]: http://blogs.atlassian.com/2013/05/alternatives-to-git-submodule-git-subtree

## Adding a new dependency

    git subtree add --prefix vendor/bar git@github.com:foo/bar master --squash

## Updating a dependency

    git subtree pull --prefix vendor/bar git@github.com:foo/bar master --squash
