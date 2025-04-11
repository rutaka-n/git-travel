# git-travel
Extension for git that allows to travel over branch commit history backward and forward easialy.

## Install
Ensure this script executable
```
$ chmod +x git-travel
```
And available in the $PATH, e.g. create a link to `/usr/bin`
```
# ln -s $PWD/git-travel /usr/bin/git-travel
```

## Usage
```
$ git travel master --help
git travel <branch name> [[ -b | --backward [ -n <N> ] ] | [ -f | --forward [ -n <N> ] ] | [ --head ] | [ --tail ]]

Travel over commit history of the branch.

OPTIONS

    -h, --help      Prints this message.

    -b, --backward  Checkout to N-th commit backward from current commit in history of the branch.

    -f, --forward   Checkout to N-th commit forward from current commit in history of the branch.

    -n <N>          Set the number of commits for go forward or backward. N equals 1 if not specified.

    --head          Checkout to HEAD of the branch - latest commit.

    --tail          Checkout to first commit of the branch.
```
