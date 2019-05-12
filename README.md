# node-red-exec-local

To execute node-red with local settings.  
Default Node-RED saves settings to user directory like ``%USERPROFILE%\.node-red``.  
This repository starts with option settings to save local directory.  

## Prepare

```sh
git clone [this repos]
cd [repos dir]
npm i
```

## Execute

```sh
npm start
```


## Portable settings

``package.json`` in this repo uses ``--settings``, ``--userDir`` and ``--flowFile`` options to run Node-RED.
The options specify location to store in your local directory.


## Debug in VS Code

For debugging purpose, this repository has ``./vscode/launch.json``.  
You can debug your code / your Node-RED execution easily in VS Code.  
launch.json also has options for portable settings.  

There's 2 way to debug.  
One is to run Node-RED in VS Code debugging feature.  
The other one is to pick up process that have already running.  

### Debug to run Node-RED

* Click debug pane on side menu.
* Select a configuration "Run Node-RED".
* Start debugging

### Debug to pick process

* Execute Node-RED e.g. ``npm start``
* Click debug pane on side menu.
* Select a configuration "Pick process".
* Start debugging
