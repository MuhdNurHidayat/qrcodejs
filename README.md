# QRCode.js
QRCode.js is javascript library for making QRCode. QRCode.js supports Cross-browser with HTML5 Canvas and table tag in DOM.
QRCode.js has no dependencies.

Project forked by Yaya MNH48 ([MuhdNurHidayat](https://github.com/MuhdNurHidayat/qrcodejs)) from Zhiyuan Ling ([zhiyuan-l](https://github.com/zhiyuan-l/qrcodejs)) to add GitHub page publishing as GitHub does not allow hotlinking from raw git files on their content delivery network. Zhiyuan Ling has forked it from [KeeeX](https://github.com/KeeeX/qrcodejs) who had [added fix for Code Length Overflow Error](https://github.com/davidshimjs/qrcodejs/pull/109) and merged the [border option](https://github.com/davidshimjs/qrcodejs/pull/54) by [nosrevi](https://github.com/nosrevi/qrcodejs/tree/border). Both KeeeX and nosrevi forked from the [original repository](https://github.com/davidshimjs/qrcodejs).

## Basic Usages
```html
<div id="qrcode"></div>
<script type="text/javascript">
new QRCode(document.getElementById("qrcode"), "https://github.com/KeeeX/qrcodejs");
</script>
```

or with some options

```html
<div id="qrcode"></div>
<script type="text/javascript">
var qrcode = new QRCode(document.getElementById("qrcode"), {
	text: "https://github.com/KeeeX/qrcodejs",
	width: 128,
	height: 128,
	border: 4,
	colorDark : "#000000",
	colorLight : "#ffffff",
	correctLevel : QRCode.CorrectLevel.H
});
</script>
```

and you can use some methods

```javascript
qrcode.clear(); // clear the code.
qrcode.makeCode("https://github.com/KeeeX"); // make another code.
```

### Other versions

#### Using with webpack (KeeeX)

```javascript
const QRCode = require("@keeex/qrcodejs-kx");
// Use QRCode as usual
```

## Browser Compatibility
IE6~10, Chrome, Firefox, Safari, Opera, Mobile Safari, Android, Windows Mobile, ETC.

## License
MIT License