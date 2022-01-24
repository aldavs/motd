# motd (message of the day)
## about
My 'message of the day' shell scripts executed at SSH login. Designed with minimal dependencies to be platform-agnostic so I don't have to modify for each deployment.
## dependencies
- [figlet](http://www.figlet.org/) (for `00-banner`)
- [hddtemp](https://savannah.nongnu.org/projects/hddtemp/) (for `36-diskstatus`)
- [smartmontools](https://www.smartmontools.org/) (for `36-diskstatus`)
- [fail2ban](https://www.fail2ban.org/wiki/index.php/Main_Page) (for `50-fail2ban`)
- [docker](https://www.docker.com/) (for `60-docker`)
## installation
1. `git clone https://github.com/aldavs/motd.git && cd motd`
2. `sudo chown root:root *`
3. `sudo cp issue* /etc/`
4. `sudo cp * /etc/update-motd.d/`
## usage
Scripts are executed at login, or can be tested via `sudo run-parts /etc/update-motd.d`.
## credits
Based on yboetz's [motd](https://github.com/yboetz/motd) repo and bcyran's [fancy-motd](https://github.com/bcyran/fancy-motd) repo which are based on u/LookAtMyKeyboard's [reddit post](https://www.reddit.com/r/unixporn/comments/8gwcti/motd_ubuntu_server_1804_lts_my_motd_scripts_for/).
