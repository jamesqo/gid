# gid

gid (aka Get It Done) is a script that adds, commits, and pushes to your Git repo in one go.

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
