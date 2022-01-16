# motd (message of the day)
## about
Collection of shell scripts executed at initial SSH connection. Designed to be platform-agnostic.
## dependencies
- [figlet](http://www.figlet.org/) (for `10-display-name`)
## usage
Copy the files to `/etc/update-motd.d/`. Set the `PrintMotd` option to `yes` in the sshd config.
