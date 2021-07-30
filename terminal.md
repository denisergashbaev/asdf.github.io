* Create host config in `home/USERNAME/.ssh/config` and use it for VSC remote development and scp
```
Host HOST_NAME
  HostName 6.tcp.ngrok.io 
  User USERNAME
  Port PORT_NUMBER
```
```bash
scp HOST_NAME:~/SOME_DIRECTORY/ local_file_name.md
```


* Check ubuntu version
```bash
lsb_release -a
```

* unzip and move to a folder
```bash
unzip package.zip -d /opt
```
