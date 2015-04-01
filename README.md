# togist

Automagically copies bash output to a new gist.

Accepts STDIN and uses bash history to figure out what commands were
executed before togist was called in the pipe chain.

## Dependencies
* GITHUB\_TOKEN environment variable (see [here](https://help.github.com/articles/creating-an-access-token-for-command-line-use/))
* curl
* jq

## Installation

For now just copy `togist` to your /usr/local/bin directory.

## Example

```bash
  echo "some output" | togist
```

This results in a new gist:

|Name|bigmac.local.1427906198.out|
|Description|echo "some output"|
|Content|some output|
