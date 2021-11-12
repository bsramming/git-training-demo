
# Command

    reset [options] 

# What It's Used For

***Be careful with this command!***

The `reset` command will undo all un-committed changes and reset your files back to the current changeset.

> Note: what I call 'current changeset' is also called 'HEAD' in git. This is simply the base set of files for your current repo. The reset command will default to this.

There are different options to this command to change what exactly gets affected. Read the official git help documentation for more details. I tend to use this command as a last resort when I know I want to start something over again.

# Options

Below are some useful options to use with the `reset` command. This is not an exhaustive list, but the ones I use most often.

| Option | Usage | 
| ---- | -----|
| --soft | Will reset all files back to current changeset. However, it will leave any changed files not committed will remain as such. |
| --hard | Will reset all files back to current changeset. Changes made to tracked files will be discarded. |

# Examples

Below are some common examples of the add command.

- I was experimenting, but the changes ultimately didn't work. Let me reset back to the changeset before starting these changes and try a different approach:

        git reset --hard
