
# Command

    commit [options]

# What It's Used For

The `commit` command is used to commit *staged* files to your *local* branch.

This command is usually ran after executing the `add` command which stages your changes. However, with the right options you can actually combine the add and commit commands together. See below.

You can execute the commit command multiple times to create more than one commit on your local branch.

Note: this command does not impact the remote repository, only your local copy. See the push command for uploading changes to the remote branch.

# Options

Below are some useful options to use with the `commit` command. This is not an exhaustive list, but the ones I use most often.

| Option | Usage | 
| ---- | -----|
| -m | This allows you to specify a message for the commit right on the command line. If this option is not provided then git will launch your default editor for you to enter the commit message. To make things easy I tend to always provide it when using commit. |
| -a | Used to also automatically stage modified files. This saves you from having to run the `add` command prior to commit. Note: This will not stage untracked files that git doesn't know about (i.e. new files you might have added). You will need to use `add` for those. |
| -am | This is simply specifying both options above. It's saying to add the files and here is the commit message. |

# Examples

Below are some common examples of the commit command.

- Add the modified files to staging and commit them to the branch. This will open up your default editor to enter a commit message.

        git commit -a

- Commit the already staged changes to the branch with the specified commit message:

        git commit -m "Added feature A to the code"

- Add the modified files to staging and commit them to the branch with the specified commit message:

        git commit -am "Adding feature B to the code"

***
[Back to Table of Contents](../TableOfContents.md)
