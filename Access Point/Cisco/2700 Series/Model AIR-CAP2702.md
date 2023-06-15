> **Note**
> Default username/password: Cisco

# Commands to update:
```
enable
```
```
debug capwap console cli
```
> **Note**
> Replace `ip` with the tftp server ip and `update.tar` with the .tar file name
```
archive download-sw /force /overwrite tftp://ip/update.tar
```

# Commands to enable Web UI:
```
enable
```
```
config t
```
> **Note**
> Replace `cisco` with any password except `Cisco`
```
enable secret cisco
```
```
ip http server
```

Enter debug mode:
```
debug capwap console cli
```

Exit debug mode:
```
undebug all
```