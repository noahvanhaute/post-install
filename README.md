# Post-install

Personal script for setting up a fresh install of openSUSE Tumbleweed.

## Perquisites

- `git` and `curl` must be installed.
- A working ssh setup for GitHub is expected by default.
- You run the script as a user.

## Usage
**! Never run a script off the internet without checking what it does first !**

This script can be ran without any cloning or downloading:
```console
curl https://raw.githubusercontent.com/noahvanhaute/post-install/refs/heads/main/post-install | bash
```
After this you will be prompted for your root password, simply enter that and wait.

Some optional flags are also provided:
```console
curl https://raw.githubusercontent.com/noahvanhaute/post-install/refs/heads/main/post-install | bash -s -- -c -n hostname -w
```

| Flag          | Action                                                                                                             |
| ------------- | ------------------------------------------------------------------------------------------------------------------ |
| `-c`          | The scrips uses ssh for cloning the dotfiles repo by default, this flag will let you use https instead.            |
| `-n hostname` | Set the hostname of the system, replace `hostname` with whatever you want (within the requirements for hostname). |
| `-w`          | Specify that the install is a WSL install.                                                                         |
