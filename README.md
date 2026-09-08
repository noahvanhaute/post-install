# Post-install

Personal script for setting up a fresh install of openSUSE Tumbleweed.
Running on a WSL install is automatically detected and necessary adjustments are made.

## Prerequisites

- `curl` must be installed.
- A working ssh setup for GitHub is expected by default.
- You run the script as a user.

## Usage

> [!WARNING]
> Never run a script off the internet without checking what it does first!

This script can be ran without any cloning or downloading:

```console
curl https://raw.githubusercontent.com/noahvanhaute/post-install/main/post-install | bash
```
After this you will be prompted for your root password, simply enter that and wait.

An optional flag is also provided to let you set the hostname of the system.

```console
curl https://raw.githubusercontent.com/noahvanhaute/post-install/main/post-install | bash \
-s -- -n coolhostname
```
