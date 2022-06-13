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

## Test
`sample/index.js` is test program. You can run the program. 
### Preparence
- Connect D'CENT hardware wallet using USB cable. If you don't have the device, you can buy it in D'CENT Store. (https://store.dcentwallet.com/)

- After connecting D'CENT Hardware wallet, power on the device and confirm user fingerprint or PIN.
### Run sample
```
git clone https://github.com/DcentWallet/dcent-cli-connector.git
cd dcent-cli-connector
npm i 
node sample/index.js
```