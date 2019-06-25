# Portable Node-RED

Execute Node-RED with local settings.  
Node-RED with default options stores settings file to user directory like ``%USERPROFILE%\.node-red``.  
This configured repository has options to store settings in local directory.  


## Prepare

```sh
git clone git@github.com:ryoichi-obara/node-red-exec-local.git
cd node-red-exec-local
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

launch.json has two options to debug.
Boths are useful for you debuuging.
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
