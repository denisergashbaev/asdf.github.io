# Visual Studio Code

`.pylintrc` file for pylint linter in VSC
<https://code.visualstudio.com/docs/python/linting#_commandline-arguments-and-configuration-files>

ignoring some rules with flake8 linter:
<https://stackoverflow.com/questions/50177173/how-do-i-get-flake8-to-reliably-ignore-rules-in-vs-code>

Pointing at source folders in VSC
based on: <https://binx.io/blog/2020/03/05/setting-python-source-folders-vscode/>

Adjust contents of `.vscode/settings.json` (or create new if does not exist): 

```json
{
    "terminal.integrated.env.osx": {
        "PYTHONPATH": "${workspaceFolder}/SOURCE_FOLDER_NAME",
    },
    "terminal.integrated.env.linux": {
        "PYTHONPATH": "${workspaceFolder}/SOURCE_FOLDER_NAME",
    },
    "terminal.integrated.env.windows": {
        "PYTHONPATH": "${workspaceFolder}/SOURCE_FOLDER_NAME",
    },
    "python.envFile": "${workspaceFolder}/.env"
}
```
and contents of `.env` in root folder of the project (create one if does not exist): 
```bash
PYTHONPATH=${PYTHONPATH}:./SelfPlay
```

## Extensions

Pylance language server for Python in VS Code.
Supposedly better features (like code completion): <https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance>

Enable Pylance in `settings.json`:

```json
{
    "python.languageServer": "Pylance",
    "python.analysis.typeCheckingMode": "strict",
}
```

## VSC hotkeys (German keyboard)

select word: `Ctrl+D`

delete line: `Ctrl+Shift+K`

open quick fix menu: `Ctrl+.`

delete a line: `SHIFT + del`

open type (symbol): `Ctrl+T` 