# Scripts

Random scripts that can be useful.

## Differ

Automatically opens or copies to clipboard a url of possys with the diff commit between branches.

usage:

interactive mode:

```
differ
```

copy to clipboard:

```
differ -c
```

fast mode without interactive mode:

```
differ --repo=api commit1 commit2
```

```
differ -c --repo=shared commit1 commit2
```

How to setup so that you can access it as a command from anywhere in the CLI.

NOTE: This is for Debian based systems

So instead of:

```
/path/to/differ.sh
```

it would be:

```
differ
```

1. Move script to a folder:

```
mv ./differ.sh ~/path/to/script-folder/differ.sh
```

2. Make script executable:

```
chmod +x ~/path/to/script-folder/differ.sh
```

3. Add to path in `~/.bashrc` for Bash or `~/.zshrc` for ZSH:

```
export PATH=~/path/to/script-folder:$PATH
```
