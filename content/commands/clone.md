
# Command

    clone <repo url> [Directory Name]

# What It's Used For

Use this command to get the repository onto your local system. One will require the right privileges in order to clone the repository successfully.

The `clone` command takes in a repository URL and an optional directory name. If no directory name is provided, then git will use the name of the repository as the directory name. To be clear, this name corresponds to the name of the directory that gets created on your *local* system.

It is handy to specify your own directory name when the name of the repository is very long. For example: *my.super.wicked.awesome.repo* might be a little cumbersome to work with in your filesystem. You can specify your directory name instead: *awesome.repo*.

# Options

There are a handful of options supported by `clone`, however they are mainly used in specific situations. For our purposes we don't need to use them.

To find more details on the options supported by `clone` you can run:

    git clone --help

# Examples

Below is an example of the clone command.

- Clone the given repository into a directory named 'gitTrainingDemo' to your system:

        git clone https://github.com/bsramming/git-training-demo.git gitTrainingDemo
