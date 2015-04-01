# to_gist

Automagically pipe bash output to a new gist.

Reads STDIN, creates a new gist, and copies the URL to your clipboard.
This bash script runs in the context of your current shell and uses
bash history to figure out which commands were executed previously
in the pipe chain before togist was executed. This is kind of like
metaprogramming in bash.

## Dependencies
* GITHUB\_TOKEN environment variable (see [here](https://help.github.com/articles/creating-an-access-token-for-command-line-use/))
* curl
* jq

## Installation

For now just copy `to_gist` to your /usr/local/bin directory.

## Example

```bash
  echo "some output" | to_gist
```

This results in a new gist being created:

> Name: bigmac.local.1427906198.out
>
> Description: echo "some output"
>
> Content: some output
