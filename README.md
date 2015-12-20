# gid

![](icons/logo.png)

gid is a script that adds, commits, and pushes to your Git repo in one go.

## Usage

```bash
gid '<your git repo>'
```

### My remote/branch isn't named origin/master.

```bash
gid -b 'your-master' -r 'your-origin'
```

### I want to force push/pull to erase any merge conflicts.

```bash
gid --force
```

### Can I specify a message without having to go through $COMMIT_EDITOR?

```bash
gid -m 'Your message'
```

#### Heck, do I even have to specify a commit message? Can't you just generate one for me?

```bash
gid --lazy # or -l for the truly indolent
```

## Supported Platforms

Any system that supports Bash should be good to go, including:

- Linux
- OS X
- Git Bash (aka MinGW)
- Cygwin

## Installing gid

Linux and OS X:

```bash
installpath='/usr/local/bin/gid' # modify as needed
curl -sSL 'https://github.com/jamesqo/gid/raw/master/gid' | sudo tee $installpath
chmod +x $installpath
```

Windows (via Cygwin or Git Bash):

```bash
curl -sSL 'https://github.com/jamesqo/gid/raw/master/install.sh' | xargs -0 bash --noprofile -c && PATH+=:~/AppData/Local/gid
```

## Contributing

Contributors are welcome! Please feel free to report bugs or make pull requests to this repo.

## License

gid is licensed under the [BSD simplified license](license.bsd).
