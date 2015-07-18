# chrome-depd

This is a fork of [dougwilson/nodejs-depd](dougwilson/nodejs-depd) to support chromeiumify 

It is required as depd uses eval and that is not allowed in chrome apps. 
This module is used by [chromiumify](https://github.com/chromiumify)
  
## Installation

```bash
$ npm install chrome-depd
```

## Usage 

This library can be used directly with your browserify builds targeting Chrome Packaged Apps. 

If you want to override a thirdparty dependancy in your builds then you use

```bash
$ browserify -r chrome-depd:depd index.js -o bundle.js
```