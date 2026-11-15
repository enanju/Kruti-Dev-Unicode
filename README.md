# Kruti Dev ⇄ Unicode Converter (JavaScript)

Convert **Kruti Dev 010** Hindi text to **Unicode** (Mangal / Noto Sans Devanagari) and back - in the browser or Node.js, with no dependencies.

**Try it online:** [Kruti Dev to Unicode Converter – SmallSEOToolsPro](https://smallseotoolspro.com/addons/krutidev-unicode-converter/)

## Features
- Kruti Dev 010 → Unicode, including the ि matra, reph (र्), half letters and common conjuncts
- Unicode → Kruti Dev for typing tests and old office documents
- Zero dependencies, works offline, ~15 KB

## Usage

### Browser
```html
<script src="krutidev.js"></script>
<script>
  KrutiDev.krutiDevToUnicode("Hkkjr");   // "भारत"
  KrutiDev.unicodeToKrutiDev("हिन्दी");  // "fgUnh"
</script>
```

### Node.js
```js
const { krutiDevToUnicode, unicodeToKrutiDev } = require('./krutidev.js');
console.log(krutiDevToUnicode('iz/kkuea=h')); // प्रधानमंत्री
```

## Test
```
node test/test.js
```

## Why Unicode?
Search engines read Kruti Dev text as random English letters ("Hkkjr"), so Hindi pages typed in Kruti Dev can't rank. Unicode text works on every phone, website and search engine. Step-by-step guide: [Kruti Dev to Unicode – how to convert](https://smallseotoolspro.com/blog/kruti-dev-to-unicode-kaise-kare).

## Credits & license
MIT. The Kruti Dev → Unicode mapping table comes from [@bharattype/hindi-transliteration](https://www.npmjs.com/package/@bharattype/hindi-transliteration) (MIT, © 2026 BharatType). The Unicode → Kruti Dev direction reverses the same table.
