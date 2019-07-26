### Bitcore P2P Cash
---
https://github.com/bitpay/bitcore/tree/master/packages/bitcore-p2p-cash

```js
var Peer = require('bitcore-p2p-cash').Peer;

var peer = new Peer({host: '127.0.0.1'});

peer.on('ready', function() {
  console.log(peer.version, peer.subversion, peer.bestHeight);
});
peer.on('disconnect', function() {
  console.log('connection closed');
});
peer.connect();

peer.on('inv', function(message) {
  // message.inventory[]
});
peer.on('tx', function(message) {
  // message.transaction
});
```

```sh
npm install bitcore-p2p-cash
```

```
```


