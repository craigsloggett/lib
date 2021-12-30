# lib

A library of POSIX shell utilities.

## Installation

1. Download the .zip file on the main page of the GitHub and extract the .zip file to your desired location.
2. (Optional) Symlink this library to your home folder for convenience:

```shell
ln -s lib ~/.local/lib/shell
```

## Usage

Import any utility found in the library in your shell script:

```shell
#!/bin/sh
#
# my_script.sh - Automate a tedious task.

# Source the logging utility.
# shellcheck source=/dev/null
. ~/.local/lib/shell/logging

# Now you have consistent logging across all of your shell scripts.
info "This is a log message."
error "Oops, something bad happened!"
```

## Contributing

Clone this repository to any directory on your system using `git`:

```shell
git clone https://github.com/craigsloggett/lib.git
```

`shellcheck` is used to ensure each utility is POSIX compliant (and therefore portable).
