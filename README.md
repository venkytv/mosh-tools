# mosh-tools
Scripts for working with mosh as an alternative to ssh

### Installation
- Copy/symlink `iterm-ssh` to a directory in your PATH
- Copy `iterm-ssh.conf` to your home directory as `~/.iterm-ssh.conf`
- Modify `~/.iterm-ssh.conf` as per your needs.

### Usage
```
$ iterm-ssh <hostname>

$ iterm-ssh --help
```

### Tips

I configure my connections to connect to a tmux session on the remote machines.
The `tmux-launch` script in `util` is copied to all my remote machines under
`~/libexec`, and my local `~/.iterm-ssh.conf` file looks like this:

```
[_defaults]
remote_command = libexec/tmux-launch
...
```
