
# Command

    config [options]

# What It's Used For

The `config` command is used for reading and updating the git config. THe git config contains various options to change the behavior of git. A few of the more useful settings I use are shown below in the examples.

Note: git has both a local repository config and a global config. The settings set below are done at the global level.

The config can also store alias commands. Think of these as shortcuts to git commands to make your life easier! See the examples below.

# Options

Below are some useful options to use with the `config` command. This is not an exhaustive list, but the ones I use most often.

| Option | Usage | 
| ---- | -----|
| --global | Read or write variables to global config. |
| --get *name* | Use to return the value of the given variable *name* |
| --list | Use to show all the config variables and their values. |
| --unset *name* | Remove the variable with the given *name* from the config |

# Examples

Below are some common examples of the COMMAND command.


- Updating or setting the user.name config property. This is the first critical config option to set! Useful to identify your commits.

        git config --global user.name "Jane Doe"

- Updating or setting the user.email config property. This is the second critical config option to set! Useful to identify your commits.

        git config --global user.email "Jane.doe@supertech.com"

- The `status` command is used a lot. I actually like `status -s` which displays a shorten version of the status output. Instead of typing *status -s* every time I can create an alias in the config such that all I have to type is: *git s*

        git config --global alias.s "status -s"

- Another useful alias is one for the `log` command. The alias below will display the repository log data in a nice graph format.

        git config --global alias.lga "log --graph --oneline --all --decorate"

- If I no longer what a variable set in the config, use --unset option to remove it:

        git config --global --unset alias.s

***
[Back to Table of Contents](../TableOfContents.md)
