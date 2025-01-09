# cleanup

Cleanup syslog:
```bash
sudo tee /var/log/syslog < /dev/null
sudo tee /var/log/syslog.1 < /dev/null
```

Clean journalctl logs:
```bash
# Retain only the past two days:
journalctl --vacuum-time=1d

# Retain only the past 500 MB:
journalctl --vacuum-size=500M
```
