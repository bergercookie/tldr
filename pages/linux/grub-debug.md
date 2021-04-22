# grub-debug

> Commands related to troubleshooting / viewing grub-specific configuration.

- View all the grub menu entries:

`awk -F\' '/menuentry / {print $2}' /boot/grub/grub.cfg`

- Update the grub menu using the entries found under `/boot`:

`sudo update-grub`

- Reboot to a specific grub entry the very next time:

`sudo grub-reboot {{N}}`
