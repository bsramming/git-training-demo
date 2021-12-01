
# Command

    log [options]

# What It's Used For

The `log` command will show the commit logs.

This command is actually very powerful in querying the commit history of your repository. By default, specifying no options, you will see the commit history. For each commit it will show:
- Commit ID
- Author - User name and email of who made the commit.
- Date - When the commit was made.
- Commit message


# Options

The `log` command has many options available to not only query different aspect of the commit history, but also change what information is returned. This guide does not go into all of those details. To learn more about all the options available for this command I encourage you to check out:

        git log --help

# Examples

Below are some common examples of the log command.

- Show the basic commit log information:

        git log

- Show a stream-lined, graph version of the log history. This is how I primarily use the log command. I even created an alias for this in my git config. See the `config` command for more details. Very useful to see the commit history at a glance.

        git log --graph --oneline --all --decorate

***
[Back to Table of Contents](../TableOfContents.md)
