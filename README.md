# to_gist

Automagically pipe bash output to a new gist.

Reads STDIN, creates a new gist, and copies the URL to your clipboard.
This bash script runs in the context of your current shell and uses
bash history to figure out which commands were executed previously
in the pipe chain before to\_gist was executed. This is kind of like
metaprogramming in bash.

## Installation

```bash
brew tap ericr/formulae
brew install to_gist
```

If you haven't already, generate a GitHUb access token for comamnd line
use. You can find more information about that [here](https://help.github.com/articles/creating-an-access-token-for-command-line-use/).

## Example

What better way to demonstrate to\_gist than with a real example? The
following generated [this gist](https://gist.github.com/91fe774c9a174befb7a1):

```bash
export GITHUB_TOKEN="...redacted..."
echo "some output" | echo "some other output" | to_gist
```
