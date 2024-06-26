# rtl-detect-intl

This is a fork of [rtl-detect](https://github.com/shadiabuhilal/rtl-detect) that uses the browser/node `Intl` API if possible: [Locale.getTextInfo()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Intl/Locale/getTextInfo#return_value)

## Usage

### require rtl-detect-intl lib
```js
var rtlDetect = require('rtl-detect-intl');
```

### isRtlLang
This function will check if the locale is right-to-left language or not.

Examples:

```js
var isRtl = rtlDetect.isRtlLang('ar-JO');
// isRtl will be true
```

```js
var isRtl = rtlDetect.isRtlLang('ar_JO');
// isRtl will be true
```

```js
var isRtl = rtlDetect.isRtlLang('ar');
// isRtl will be true
```

```js
var isRtl = rtlDetect.isRtlLang('en-US');
// isRtl will be false
```

### getLangDir
This function will get language direction for the locale.

Examples:

```js
var langDir = rtlDetect.getLangDir('ar-JO');
// langDir will be 'rtl'
```

```js
var langDir = rtlDetect.getLangDir('ar_JO');
// langDir will be 'rtl'
```

```js
var langDir = rtlDetect.getLangDir('ar');
// langDir will be 'rtl'
```

```js
var langDir = rtlDetect.getLangDir('en-US');
// langDir will be 'ltr'
```

Copyright 2015, Yahoo! Inc.
