# test react update

This is build for spike the [issue](https://github.com/sanniassin/react-input-mask/issues/39) of update react from v0.13 to v15.0 with [react-input-mask](https://github.com/sanniassin/react-input-mask)

And with this project I found that with react-router@0.13, the update `npm i react@15.0 --save` will fail with the following message:

```
npm WARN package.json test-react-update@1.0.0 No description
npm WARN package.json test-react-update@1.0.0 No repository field.
npm WARN package.json test-react-update@1.0.0 No README data
npm ERR! Darwin 15.4.0
npm ERR! argv "/Users/jwqin/.nvm/versions/node/v4.2.1/bin/node" "/Users/jwqin/.nvm/versions/node/v4.2.1/bin/npm" "i" "react@15.0" "--save"
npm ERR! node v4.2.1
npm ERR! npm  v2.15.6
npm ERR! code EPEERINVALID

npm ERR! peerinvalid The package react@15.0.2 does not satisfy its siblings' peerDependencies requirements!
npm ERR! peerinvalid Peer react-input-mask@0.6.7 wants react@>=0.12.0
npm ERR! peerinvalid Peer react-router@0.13.5 wants react@0.13.x||0.14.x

npm ERR! Please include the following file with any support request:
npm ERR!     /Users/jwqin/workspace/test-react-update/npm-debug.log
```

And when remove react-router, the update can run successfullly.
