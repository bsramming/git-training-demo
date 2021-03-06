
# Command

    checkout [options] <branchName | commit ID>

# What It's Used For

The `checkout` command is used primarily for switching between branches. The 4 primary tasks are:
1. Switching between different branches on your local repository copy.
2. Creating a new local branch.
3. Going back in time to a specific commit ID.
4. Undoing changes to a specific file.

# Options

Below are some useful options to use with the `checkout` command. This is not an exhaustive list, but the ones I use most often.

| Option | Usage | 
| ---- | -----|
| -b | Use to create a new local branch and check it out (i.e. make it the active branch). |

# Examples

Below are some common examples of the `checkout` command.

- Create a new local branch and make it active:

        git checkout -b myAwesomeBranch

- Switch to the *main* branch. Note: *main* branch is usually a standard branch in GitHub. Other git platforms might use *master*.

        git checkout main

- Switch to a specific commit ID. Note: each commit has a unique ID. It is a long hex string auto-generated by git. You can use the `log` command to see them.

        git checkout 323666a19846652190c25379bdc4f928b439803e

- Made some changes to the checkout.md file that I no longer need. To undo those changes:

        git checkout -- content/commands/checkout.md

***
[Back to Table of Contents](../TableOfContents.md)
