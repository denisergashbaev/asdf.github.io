# bash

`ssh and cd` in one command:

```bash
my-ssh () { ssh "USER_NAME@SERVER_NAME" -p PORT_NO -t "cd \"$1\"; exec \$SHELL -l"; }
```
