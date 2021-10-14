# ES6 JavaScript Snippets for Visual Studio Code

<!-- markdownlint-disable MD033 -->

<p>
  <a href="https://marketplace.visualstudio.com/items?itemName=Cjay.es6-javascript-snippets">
    <img src="https://vsmarketplacebadge.apphb.com/version-short/Cjay.es6-javascript-snippets.svg">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=Cjay.es6-javascript-snippets">
    <img src="https://vsmarketplacebadge.apphb.com/installs/Cjay.es6-javascript-snippets.svg">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=Cjay.es6-javascript-snippets">
    <img src="https://vsmarketplacebadge.apphb.com/downloads-short/Cjay.es6-javascript-snippets.svg">
  </a>
</p>

[This extension](https://github.com/Chris56974/ES6-JavaScript-Snippets) (which can also be found on the [marketplace](https://marketplace.visualstudio.com/items?itemName=Cjay.es6-javascript-snippets)) is a JS snippets pack largely inspired by other extensions ([Charalampos Karypidis](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets)) but with a few of my own twists and added snippets. I use [vim extension](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim) so my snippets is likely biased towards vim users (I use "o"/"O" & "j"/"k" to jump around).

<a href="https://imgflip.com/gif/3489ko"><img src="https://i.imgflip.com/3489ko.gif" title="made at imgflip.com" alt="demonstration of the JS snippets plugin"/></a>

## Supported File Types

- JavaScript (.js)
- TypeScript (.ts)
- JavaScript React (.jsx)
- TypeScript React (.tsx)
- Html (.html)
- Vue (.vue) (Vetur extension required)

### Help

1. You use each snippet by typing out their name (i.e. req) and then hitting TAB on your keyboard.
2. You must be in one of the supported file types for these snippets to work.
3. Some snippets have multiple steps you can cycle through.

- Hitting TAB will move you forward one step
- Hitting CTRL + TAB will move you back one step
- If you can't see any suggested snippets try hitting CTRL/COMMAND + SPACE

`$1` is where the snippet starts and `$0` is where the snippet ends.

## Snippets

```js
// CommonJS
const $0 = require('$1'); // req
module.exports = $0;      // mex

// ES6
import $0 from '$1';            // imp
import '$0';                    // imn
import { $0 } from '$1';        // imd
import * as $1 from '$0';       // ime
import { $2 as $0 } from '$1';  // ima
export default $0;              // exp
export function $0() {}         // exf
export function $1($0) {}       // exfn
export { $0 } from '$1'         // exd
export { $2 as $0 } from '$1';  // exa

// Console
console.log()          // cl
console.log("$1", $1)  // clo
console.dir($1)        // cdir

// DOM
addEventListener('$1', $0)  // ae
querySelector('$0')         // qs
querySelectorAll('$0');     // qsa
appendChild($0);            // ac
removeChild($0);            // rc
createElement($0);          // ce
createTextNode($0);         // ctn
createDocumentFragment();   // cdf
classList.add($0);          // ca
classList.toggle($0);       // ct
classList.remove($0);       // cr
getElementById($0);         // gi
getElementsByClassName($0); // gc
getElementsByTagName($0);   // gt
getAttribute($0);           // ga
setAttribute($0);           // sa
removeAttribute($0);        // ra
querySelector('$1').addEventListener('$2', $0) // qsae

forEach(($1) => { $0 })     // fe
for (const $1 of $2) { $0 } // fof
for (const $1 in $2) { $0 } // fin

function $0() {}       // fn
function $1($0) { }    // fnn
const $1 = ($2) => $0  // afn
const $1 = ($0) => {}  // afnn

const { $0 } = $1 // dob
const [$0] = $1   // dar

prototype.$1 = $0   // proto
(($1) => { $0 })(); // iife

// cla1, cla2, cla3 (for 1, 2 or 3 properties)
class $1 {
  constructor($2) {
    this.$2 = $2;
  }
}

// clex
class ${1:className} extends ${2:parentClass} {
  constructor($0) {
    super();
  }
}

constructor($0) {}  // con

$1 ($2) { $0 }               // met
get $1 () {return this.${0}} // pget
set $1 (${2:value}) {${0}}   // pset

setInterval(() => { $0 }, $1);  // sti
setTimeout(() => { $0 }, $1);   // sto

JSON.parse($0);     // jp
JSON.stringify($0); // js

return new Promise((resolve, reject) => { $0 }); // prom

// cmmb
/**
|--------------------------------
| $0
|--------------------------------
*/
```

## [MIT License](https://github.com/Chris56974/ES6-JavaScript-Snippets/blob/master/LICENSE)
