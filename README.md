# Create

A simple bash script to create web apps that can be installed on devices as progressive web apps (pwa).

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

## Files created

[index.html](myAwesomeProject/index.html)  
[css/main.css](myAwesomeProject/css/main.css)  
[js/main.js](myAwesomeProject/js/main.js)  
[sw.js](myAwesomeProject/sw.js)  
[favicon.png](myAwesomeProject/favicon.png)  
[manifest.appcache](myAwesomeProject/manifest.appcache)  
[manifest.json](myAwesomeProject/manifest.json)  

## Bugs

There's a discussion about who should be in charge of the cache (for offline disponibility). Some say the responsable should be the manifest.appcache (which works, but don't prompt the user to install the app) - others say the cache should be done on the service worker script (that is giving me a headache). Soon as possible I'll try to figure this out.
