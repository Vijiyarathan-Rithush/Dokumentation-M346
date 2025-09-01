
#### Passwörter
```pwd
Riethuesli>12345
```

---
# 1. Hole die VM's

## LP-22.04
```pfad
C:\VMs\LP-22.04
```

## LF-2.25
```pfad
C:\VMs\LF_2.25\LF_2.25
```

## WP1-22h2
```pfad
C:\VMs\WP1-22H2
```

---

# 2. IP Adresse bestimmen und Pingen

1. IP Adresse des Routers holen
2. IP Adresse von Ubuntu VM holen (ens33)

```ip
192.168.210.22
```

3. IP Adresse von Windows VM holen

```ip
182.168.210.132
```

### Befehle:
```windows
ping 192.168.210.22
```

```linux
ping www.gbssg.ch
```

---

# 3. SSH-Server download

```linux
sudo apt-get update
```

```linux
sudo apt install openssh-server -y
```

```linux
sudo service ssh status
```

---

# 4. SSH-Verbindung mit Passwort

```ssh
ssh-keygen
```

```windows
ssh vmadmin@192.168.210.222
```

---

# 5. SSH-Verbindung mit publickey

Gebe folgenden Befehl ein:

```windows
scp C:\Users\vmadmin\.ssh\id_rsa.pub vmadmin@192.168.210.22:~/.ssh/authorized_keys
```

---

# 6. Testen und Zugang

```windows
ssh -i C:\Users\vmadmin\.ssh\id_rsa vmadmin@192.168.210.22
```

---

# 7. Passwort deaktivieren

```linux
sudo nano /etc/ssh/sshd_config
```

Suche nach **PasswordAuthentication** und entferne den #

Danach Service neustarten

```linux
sudo service ssh restart
```
