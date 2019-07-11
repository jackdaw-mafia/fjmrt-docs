# How to use QR codes

https://www.npmjs.com/package/react-native-qrcode

1. npm i react-native-qrcode
2. insert the following onto page: 
```<QRCode
          value={this.state.text}
          size={200}
          bgColor='purple'
          fgColor='white'/>```
3. for each deal give value=coupon ID
4. when scanning the QR code check that code = couponID for that deal
