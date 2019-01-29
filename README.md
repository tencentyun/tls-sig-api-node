## npm 集成
```shell 
npm install tls-sig-api
```

## 接口调用
```javascript
var sig = require('tls-sig-api');
var config = {
    "sdk_appid": 1400000000,
    "expire_after": 180 * 24 * 3600,
    "private_key": "ec_key.pem",
    "public_key": "public.pem"
}

var sig = new sig.Sig(config);
console.log(sig.genSig("xiaojun"));
```
