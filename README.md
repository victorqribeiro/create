# Create

A simple bash script to create web apps.

## About

This is a very simple but very useful script to create a web app template. For Chrome to consider your web app a valid app, it needs to have a cache manifest, a web app manifest, a bigger than 144x144 pixel favicon and a registered service worker (read more about it [here](https://developers.google.com/web/tools/lighthouse/audits/install-prompt)). This script takes care of it for you.

## How to use

Put it in your scrips folder.

Give it execute permisson
```
chmod +x create
```

Run it with a project's name as argument
```
create myAwesomeProject
```

Done!

## Project tree
```
myAwesomeProject
 |-- css
 |   '-- main.css
 |-- js
 |   '-- main.js
 |-- index.html
 |-- sw.js
 |-- favicon.png
 |-- manifest.appcache
 |-- manifest.json
```
