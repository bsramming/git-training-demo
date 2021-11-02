
# Command

    status [options]

# What It's Used For

The `status` command shows the changes made to the files in your current local branch. For example, it will report back files that have been modified but not staged, staged files, and files that are not tracked.

Note: there is a special file named .gitignore that can affect the output of this command. This file specifies filename patterns that you do not want to be tracked by your git repository. For example, the compiled .obj files from a C++ project are created every time your project is built. Therefore these files do not need to be tracked in the repo. By specifying '*.obj' in the .gitignore file, these will not show up in the `status` command output.

# Options

Below are some useful options to use with the `status` command. This is not an exhaustive list, but the ones I use most often.

| Option | Usage | 
| ---- | -----|
| -s | This will display the status output in short format. Will only show list of file changes and not the git command suggestions. |

# Examples

Below are some common examples of the status command.

- Show the current repo file status:

        git status

- Show the current repo file status in short format:

        git status -s
