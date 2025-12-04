# Example of showing credentials in a Git Repository

Github finds commit hashes starting with the first 4 characters.

This means that guessing commit hashes becomes much easier, as it is not necessary to guess all 40 characters of the commit.

In addition, deleted commits are also available in the Github history. Here you can see an example of a deleted commit (overwritten via force push) that can still be found with 4 characters.
[42d6](https://github.com/marcelthole/git-leak-example/commit/42d6) instead of the full commit hash [42d6813b35ed820c76da29498e53c9569eb1d46f](https://github.com/marcelthole/git-leak-example/commit/42d6813b35ed820c76da29498e53c9569eb1d46f)

## Solution for unwanted commits
First of all, change your credentials in any case. After that you could use `git-filter-branch` or a tool like https://github.com/rtyley/bfg-repo-cleaner to delete the file completly.