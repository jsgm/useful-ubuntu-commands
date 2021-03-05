# useful-ubuntu-commands

**Restart PHP-FPM with Plesk**
```bash
service plesk-php74-fpm restart
service plesk-php71-fpm restart
```

**Kill all PHP processes**
```bash
kill $(ps aux | grep '[p]hp' | awk '{print $2}')
```

**Check free RAM memory**
```bash
free -m
```

**Disk usage**
```bash
df -h
```

**Delete logs files older than X days**
```bash
journalctl --vacuum-time=10d
```

**Change user home**
```bash
cd /home;
sudo mkdir [folder]
sudo chown [username]:[username] [folder]
sudo usermod -d [folder] [username]
```
