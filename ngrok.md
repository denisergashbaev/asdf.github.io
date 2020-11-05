# ngrok

Starting ngrok tunnels defined in config file

```bash
./ngrok start --config=my-tunnel-config.yml [--all or TUNNEL_NAME]
```

Example tunnel file `my-config.yml`

```yml
authtoken: YOUR_SECRET_TOKEN
tunnels:
   tensorboard:
      proto: http
      addr: 6006
   remotedev:
      proto: tcp
      addr: 22
```
