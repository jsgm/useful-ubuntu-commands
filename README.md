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

**Check server uptime**
```bash
uptime
```

**Disk usage**
```bash
df -h
```

**Delete logs files older than X days**
```bash
journalctl --vacuum-time=10d
```

**Change the owner of a folder**
```bash
sudo chown -R [username]:[username] [folder]
(-R) recursive
```

**Set WordPress correct permissions**
```bash
sudo chown -R www-data:www-data [folder]
cd [folder]
find . -type d -exec chmod 755 {} \;  # Change directory permissions rwxr-xr-x
find . -type f -exec chmod 644 {} \;  # Change file permissions rw-r--r--
```

**Change user home**
```bash
cd /home;
sudo mkdir [folder]
sudo chown [username]:[username] [folder]
sudo usermod -d [folder] [username]
```

**Extract tar file**
```bash
tar -zxvf [file]
```
