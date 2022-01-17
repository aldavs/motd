# motd (message of the day)
## about
Collection of shell scripts executed at initial SSH connection. Designed to be platform-agnostic.
## dependencies
- [figlet](http://www.figlet.org/) (for `10-display-name`)
- [hddtemp](https://savannah.nongnu.org/projects/hddtemp/) (for `36-diskstatus`)
## usage
Copy the files to `/etc/update-motd.d`.
Scripts are executed at login, or can be tested via `sudo run-parts /etc/update-motd.d`.
## credits
Based on yboetz's [motd](https://github.com/yboetz/motd) repo and bcyran's [fancy-motd](https://github.com/bcyran/fancy-motd) repo.
