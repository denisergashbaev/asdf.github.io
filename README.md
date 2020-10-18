# pyCharm hotkeys

Alt+1: switch to Project view

Ctrl+Shift+I: Quick definition of a method/class

Ctrl+Shift+E: Recent locations

Ctrl+U: Go to definition

Ctrl + Alt + o: Optimize imports

# VSC

`.pylintrc` file for pylint linter in VSC 
https://code.visualstudio.com/docs/python/linting#_commandline-arguments-and-configuration-files

# bash 

`ssh and cd` in one command: 
```bash 
my-ssh () { ssh "USER_NAME@SERVER_NAME" -p PORT_NO -t "cd \"$1\"; exec \$SHELL -l"; }`