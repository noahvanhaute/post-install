# Post-install

Personal script for setting up a fresh install of openSUSE Tumbleweed.

## Perquisites

- `git` must be installed
- A working ssh setup for GitHub is expected by default

## Usage

This script can be ran without any cloning or downloading:
```console
curl https://raw.githubusercontent.com/noahvanhaute/post-install/refs/heads/main/post-install | bash
```

The script also supports some flags:
```console
curl https://raw.githubusercontent.com/noahvanhaute/post-install/refs/heads/main/post-install | bash -s -- -c -n hostname -w
```

| Flag          | Action                                                                                                             |
| ------------- | ------------------------------------------------------------------------------------------------------------------ |
| `-c`          | The scrips uses ssh for cloning the dotfiles repo by default, this flag will let you use https instead.            |
| `-n hostname` | Set the hostname of the system, replace `hostname` with whaterver you want (within the requirements for hostname). |
| `-w`          | Specify that the install is a WSL install.                                                                         |
