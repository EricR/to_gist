# to_gist

Automagically pipe bash output to a new gist.

Reads STDIN, creates a new gist, and copies the URL to your clipboard.
This bash script runs in the context of your current shell, and uses
bash history to figure out which commands were executed previously
in the pipe chain before to\_gist was executed.

![](http://ericrafaloff.com/images/to_gist.gif)

## Installation

```bash
brew tap ericr/formulae
brew install to_gist
```

If you haven't already, generate a GitHUb access token for command line
use. You can find more information about that [here](https://help.github.com/articles/creating-an-access-token-for-command-line-use/).
