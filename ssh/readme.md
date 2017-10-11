# Keep alive session

If you do not setup a keep alive, most SSH sessions will close
automatically after a relatively short duration of inactivity. To fix
this, add the following to either `/etc/ssh/ssh_config` or
`~/.ssh/config`:

```bash
Host *
  ServerAliveInterval 30
  ServerAliveCountMax 3
```

Where `ServiceAliveInterval` sets the interval, in seconds, at which to
send a keep alive ping, and `ServerAliveCountMax` sets the number of
times to try the server before timing out.

**Reference:** [How to Keep Alive SSH  Sessions](https://patrickmn.com/aside/how-to-keep-alive-ssh-sessions/)
