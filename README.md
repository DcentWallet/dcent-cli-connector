# dcent-cli-connector
This is SDK for connecting D'CENT biometric wallet.<br>
`dcent-cli-connector` is modules for easy integration of D'CENT into 3rd party services.<br>

- [Integration](doc/index.md)

## Installation

### Node.js 
```
npm i dcent-cli-connector
```

## Useage

```js
// in Node.js
const DcentCLIConnector = require('dcent-cli-connector')

var result
try{
    DcentCLIConnector.initialize()
    result = await DcentCLIConnector.info()
    console.log('DcentConnector.info result - ', result)

}catch(e){
    result = e
}
DcentCLIConnector.finalize() // 
```
