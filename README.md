# aurelia-obfuscator-io-broken
Reproducing bug where Aurelia project build is broken when webpack-obfuscator is utilized.

To run, may need to install the aurelia-cli globally (details here: https://aurelia.io/docs/cli/basics#machine-setup):
```
npm install aurelia-cli -g
```

Run locally (port 8080) with:
```
au run
```

The bug should be apparent as-is (the app shouldn't build).
Comment-out the code relevant to JavaScriptObfuscator in webpack.config.js (line 6 and line 125) to build and run successfully.

I'm running node v10.15.3 on my machine.
