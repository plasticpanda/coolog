Coolog
======

Colourful logging in node.js


## Install ##

```bash
npm -S install coolog
```


## Use ##

```js
var coolog = require('coolog')
  , logger = coolog.logger('main.js', true /* don't be verbose */);
  
  
coolog.on('log', function () {
  // Global event handler
  console.log(arguments);
});
  
logger.log('Message or obj', ...);
logger.error('Message or obj', ...);
logger.warn('Message or obj', ...);
logger.info('Message or obj', ...);
logger.debug('Message or obj', ...);
logger.ok('Message or obj', ...);
```


See [this gist](https://gist.github.com/lusentis/5957823) for Logentries integration.
