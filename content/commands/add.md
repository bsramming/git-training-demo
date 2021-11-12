
# Command

    add [options] file1 file2 ...

# What It's Used For

The `add` command will add the specified files to staging. This is done before running the *commit* command.

# Options

Below are some useful options to use with the `add` command. This is not an exhaustive list, but the ones I use most often.

| Option | Usage | 
| ---- | -----|
| -A | Add all modified and untracked files to staging. |
| -n | This does a dry-run. No files are actually added, but will show what files would be added.

# Examples

Below are some common examples of the add command.

- To add the *add.md* file in the *commands* directory to staging:

        git add commands/add.md

- To add all modified, and untracked files to staging:

        git add -A

- To see what files would be added to staging without actually staging them - in other words - a dry-run. This is handy when you want to make sure your .gitignore file is accurate.

        git add -A -n
    

