## Dokumentasi Remote VM GCP

### Set up firewall 
 
 ```
 ip range 0.0.0.0/0
 tag ssh (optional)
 protocol allow-all
 ```

### Create VM

```
create vm seperti biasanya (allow http dan https network dikasih tag ssh)
```

### Edit sshd

```
sudo su -
nano /etc/ssh/sshd_config
systemctl restart sshd
passwd 

```
masukan password utk root 

### contoh sshd_config
https://raw.githubusercontent.com/EPX-PANCA/gcp-vm-remote-ssh/main/sshd_config
