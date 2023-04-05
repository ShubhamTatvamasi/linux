# freeze

Install LightDM display manager:
```bash
sudo apt install lightdm
```

Change display manager to **lightdm**:
```bash
sudo dpkg-reconfigure gdm3
```

Check the display-manager status:
```bash
systemctl status display-manager
```

Verify that your display manager has changed to `/usr/sbin/lightdm`:
```bash
cat /etc/X11/default-display-manager
```
