# Set up in VScode

## Install the following extendsion in VScode

```console
ms-python.python
ms-toolsai.jupyter
Ikuyadeu.r
donjayamanne.python-environment-manager
```

## Add the following settings to your working directory

1. Create folder called ```.vscode```
2. Create file called ```settings.json```
3. edit ```settings.json``` with the following

    ```json
    {
        "r.source.focus": "terminal",
        "r.rterm.linux": "/home/xxx/anaconda3/envs/r_env/bin/radian",
        "r.rpath.linux": "/home/xxx/anaconda3/envs/r_env/lib/R/bin",

        "r.bracketedPaste": true,
        "r.lsp.debug": true,
        "r.lsp.diagnostics": false,
        "r.rterm.option": ["--no-site-file"],
        "r.sessionWatcher": true,
        "r.source.encoding": ""
    }
    ```

4. Change the setting for ```r.rterm.linux``` and ```r.rpath.linux``` to windows or mac if you are not using linux, also update the path to your R and Radian path.

## Create New Blank Notebook

1. ```ctrl``` + ```shift``` + ```p```
2. Jupyter: Create New Blank Notebook
3. Click on the button right below ellipsis in upper right corner to choose kernel
4. Choose the one with R installed, e.g. ```R ~/anaconda3/envs/r_env/lib/R/bin/R Jupyter kernel``` or just ```R R Jupyter kernel```