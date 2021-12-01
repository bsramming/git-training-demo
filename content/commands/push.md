
# Command

    push [options]

# What It's Used For

The `push` command is used to update your remote branch with any commits made to your local branch.

This command is usually ran after executing the `commit` command.

The first time you run the `push` command on a local repository you actually need to set it up as a remote branch. To do that you will specify the *--set-upstream* option.

# Options

Below are some useful options to use with the `push` command. This is not an exhaustive list, but the ones I use most often.

| Option | Usage | 
| ---- | -----|
| --set-upstream origin (local_branch_name) | This will make the local branch with *local_branch_name* a remote branch. This needs to be set the first time one pushes to the branch. Assumes *origin* is the remote repository. This is usually default. |

# Examples

Below are some common examples of the push command.

- Make *myAwesomeBranch* a remote branch and push the local commits to it.

        git push --set-upstream origin myAwesomeBranch

- Push commits to a pre-existing remote branch:

        git push

***
[Back to Table of Contents](../TableOfContents.md)
