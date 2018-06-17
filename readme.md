_Github Tools_ provide a set of utilities that will allow you to easily manage
repositories you clone from github to your local hard drive.

# Get started
Go to the folder in which you put all repositories you clone from github, and
run the following command, to clone this repository tools, to your directory.

```
$ git clone https://github.com/rusavi/github-tools .
```

# Clone

use `./clone -u https://github.com/username/repository` to clone a new repository
to your local hard drive, this command, will first check if repository exists,
if not it will extract the `username` from the url, and create a folder with
that name, then it will clone the repository inside that folder.

# Update

When you want to update all repositories, run `./update`.

This command will first check to see if you have made any changes in the
repository, if so it will run `git fetch --all`, and if there is no changes
it will run `git pull --all`.

# List

Simply run `./list` to list all the repositories, including last commit id,
last relative update time, last user and email who made the commit, and the
commit message.

Example output:

```
danistefanovic/build-your-own-x     b978bec - 3 days ago - Daniel Stefanovic <daniel.stefanovic@gmail.com> - Merge pull request #192 from parmort/master
docker-stacks                       03b897d - 4 days ago - Peter Parente <parente@cs.unc.edu> - [ci skip] Add source-to-image alternative
dylanaraps/pure-bash-bible          04bb481 - 19 hours ago - Dylan Araps <dylan.araps@gmail.com> - Added note about binary files
externalist/exploit_playground      a8aa852 - 9 hours ago - externalist <wringer@paran.com> - - Fixed the kmsg explanation part
facebook/react                      ae14317d6 - 2 days ago - Dan Abramov <dan.abramov@gmail.com> - Inline fbjs/lib/emptyFunction (#13054)
google/gif-for-cli                  2fc0b21 - 2 days ago - Sean Hayes <sth@google.com> - Fixed export console output.
```

# Trending

Run `./trending` to clone all github trending repositories to your local hard drive.
