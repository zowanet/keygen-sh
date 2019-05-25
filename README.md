# keygen

A convenience wrapper around `ssh-keygen` for generating [Ed25519](https://en.wikipedia.org/wiki/EdDSA#Ed25519) keys with 100 KDF rounds for increased brute-force attack resistance.

## Installation

Clone this repository, then run `./install`.
The script will be symlinked into your `~/bin/` directory.

To update, run `git fetch origin && git pull origin master`.

## Usage

```bash
keygen
```
> Outputs
>
>     Usage: keygen USER[@HOST]

Requires existing target directory `~/.ssh/keys/`; saves keys as `user@host_ed25519_{private,public}_OpenSSH`.
