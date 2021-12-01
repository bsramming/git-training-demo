
# Command

    diff [files]

# What It's Used For

The `diff` command will show the changes made to the tracked files. You can limit which files are checked by listing them after the command. By default the command will diff all modified files.

This command is very useful to double check your changes before committing them to the repository. However, it can be a little hard to read when there are significant changes.

# Options

I primarily use this command without any options. To find more details on the options supported by `diff` you can run:

    git diff --help

# Examples

Below are some common examples of the diff command.

- Lets see what changes I made before commit:

        git diff

- What changes did I make to the *diff.md* file

        git diff content/commands/diff.md

***
[Back to Table of Contents](../TableOfContents.md)
