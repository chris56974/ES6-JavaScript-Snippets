## ES6 JavaScript Snippets for Visual Studio Code 

A JS snippets pack largely inspired by other snippet extensions on VSCode (Charalampos Karypidis, Mahmoud Ali, Dsznajder) but with a few of my own twists and added snippets !! :)

<a href="https://imgflip.com/gif/3489ko"><img src="https://i.imgflip.com/3489ko.gif" title="made at imgflip.com"/></a>

##### Supported languages (file extensions)

- JavaScript (.js)
- TypeScript (.ts)
- JavaScript React (.jsx)
- TypeScript React (.tsx)
- Html (.html)
- Vue (.vue) (Vetur extension required)

##### Hints
1. `control/command + space` loads the snippet suggestions if they aren't shown right away.
2. `${1}` is where the snippet starts. `$0` is where the snippet ends.
3. Press `tab` to move onto the next part of a snippet.
___
## - Imports and Exports -
#### [req] require (Common JS)
```javascript
const ${1:package} = require('${1:package}');$0
```
#### [reqq] alternative require (Common JS)
```javascript
const ${1:package} = require('${2:filePath}');$0
```
#### [mex] module exports (Common JS)
```javascript
module.exports = {$0};
```
#### [imp] import
```javascript
import ${1:moduleName} from '${2:module}';$0
```
#### [imn] import without module name
```javascript
import '${1:module}';$0
```
#### [imd] import destructuring
```javascript
import { ${1} } from '${2:module};'$0
```
#### [ime] import everything as
```javascript
import * as ${1:alias} from '${2:module}';$0
```
#### [ima] import as
```javascript
import { ${1:originalName} as ${2:alias} } from '${3:module}';$0
```
#### [exp] export default
```javascript
export default $1$0
```
#### [exd] export destructuring
```javascript
export { ${1} } from '${2:module}'$0
```
#### [exa] export as
```javascript
export { ${1:originalName} as ${2:alias} } from '${3:module}';$0
```
#### [enf] export named function
```javascript
export const ${1:functionName} = (${2:params}) => {$0};
```
#### [edf] export default function
```javascript
export default (${1:params}) => {$0};
```
#### [ecl] export class
```javascript
export default class ${1:className};$0
```
#### [ece] export class extends
```javascript
export default class ${1:className} extends ${2:baseclassName};$0
```
## - Console logging - 
#### [cas] console.assert
```javascript
console.assert(${1:expression}, ${2:object})
```
#### [ccl] console.clear
```javascript
console.clear()
```
#### [cco] console.count
```javascript
console.count(${1:label})
```
#### [cdi] console.dir
```javascript
console.dir(${1});
```
#### [cer] console.error
```javascript
console.error(${1});
```
#### [cgr] console.group
```javascript
console.group(\"${1:label}\")
```
#### [cge] console.groupEnd
```javascript
console.groupEnd()
```
#### [ci] console.info
```javascript
console.info(${1});
```
#### [cl] console.log
```javascript
console.log(${1});
```
#### [clo] console.logObject
```javascript
console.log('${1:object}', ${1:object})
```
#### [cloo] alternative console.logObject
```javascript
console.log('${1:object}', ${1:object})
```
#### [ctr] console.trace
```javascript
console.trace(${1:object})
```
#### [ctm] console.time
```javascript
console.time('${1:object}')
```
#### [cte] console.timeEnd
```javascript
console.timeEnd('${1:object}')
```
#### [clt] console.table
```javascript
console.table(${1:object});
```
#### [clt] console.table
```javascript
console.table(${1:object});
```
#### [cw] console.warn
```javascript
console.warn(${1:object})
```
#### [de] debugger
```javascript
debugger;
```
## - DOM -
#### [ae] addEventListener
```javascript
${1:document}.addEventListener('${2:load}', ${3:()} => {
   $0
});
```
#### [qs] querySelector
```javascript
${1:document}.querySelector('${2:selector}');$0
```
#### [qsae] querySelect + addEventListener
```javascript
${1:document}.querySelector('${2:selector}').addEventListener('${3:load}', ${4:()} => {
    $0
});
```
#### [qsa] querySelectorAll
```javascript
${1:document}.querySelectorAll('${2:selector}');$0
```
#### [ac] appendChild
```javascript
${1:document}.appendChild(${2:elem});$0
```
#### [rc] removeChild
```javascript
${1:document}.removeChild(${2:elem});$0
```
#### [ce] createElement
```javascript
${1:document}.createElement(${2:elem});$0
```
#### [ctn] createTextNode
```javascript
${1:document}.createTextNode('$2');$0
```
#### [cdf] createDocumentFragment
```javascript
${1:document}.createDocumentFragment()$0;
```
#### [ca] classList.add
```javascript
${1:document}.classList.add('${2:class}');$0
```
#### [ct] classList.toggle
```javascript
${1:document}.classList.toggle('${2:class}');
```
#### [cr] classList.remove
```javascript
${1:document}.classList.remove('${2:class}');
```
#### [gi] getElementById
```javascript
${1:document}.getElementById('${2:id}');
```
#### [gc] getElementsByClassName
```javascript
${1:document}.getElementsByClassName('${2:class}');
```
#### [gt] getElementsByTagName
```javascript
${1:document}.getElementsByTagName('${2:tag}');
```
#### [ga] getAttribute
```javascript
${1:document}.getAttribute('${2:attr}');
```
#### [sa] setAttribute
```javascript
${1:document}.setAttribute('${2:attr}', ${3:value});
```
#### [ra] removeAttribute
```javascript
${1:document}.removeAttribute('${2:attr}');
```
#### [ih] innerHTML
```javascript
${1:document}.innerHTML = '${2:elem}';
```
#### [tc] textContent
```javascript
${1:document}.textContent = '${2:content}';
```
## - Loops -
#### [fe] forEach
```javascript
${1:array}.forEach(function(item) {
  ${2:// body}
});
```
#### [fof] forOf
```javascript
${1:array}.forEach(function(item) {
  ${2:// body}
});
```
#### [fin] forIn
```javascript
${1:array}.forEach(function(item) {
  ${2:// body}
});
```
## - Functions -
#### [afn] anonymous function
```javascript
(${1:arguments}) => {
  ${2:// body}
}
```
#### [fn] single line function
```javascript
const ${1:methodName} = ${2:arg} => {$3}
```
#### [fnn] single line function
```javascript
const ${1:methodName} = (${2:args}) => {
  $0
}
```
#### [pr] prototype
```javascript
${1:object}.prototype.${2:method} = function(${3:arguments}) {
  ${4:// body}
}
```
#### [iife] immediately-invoked function expression
```javascript
(($1) => {
  $0
})($1);
```
#### [es5iife] immediately-invoked function expression (ES5)
```javascript
(function ($1) {
  $0
})($1);
```
#### [call] function call
```javascript
${1:method}.call(${2:context}, ${3:arguments})
```
#### [apply] function apply
```javascript
${1:method}.apply(${2:context}, [${3:arguments}])
```
#### [ofn] function as a property of an object
```javascript
${1:functionName}: function(${2:arguments}) {
	${3:// body}
}
```
#### [si] setInterval
```javascript
setInterval(function() {
	${0:// body}
}, ${1:1000});
```
#### [st] setTimeout
```javascript
setTimeout(function() {
	${0:// body}
}, ${1:1000});
```
## - JSON -
#### [jp] JSON.parse
```javascript
JSON.parse(${1:obj});
```
#### [js] JSON.stringify
```javascript
JSON.stringify(${1:obj});
```
## - Asynchronous -
#### [prom] promise
```javascript
return new Promise((resolve, reject) => {${1});
```
#### [thenc] then / catch
```javascript
.then((${1:result}) => {${2}}).catch((${3:err}) => {${4}};
```
#### [promtc] promise with then catch
```javascript
const promise = new Promise((resolve, reject) => {
  $1
}).then((${2:result}) => {
  $3
}).catch((${4:err}) => {
  $5
});$0",
```
#### [fetchget] simple fetch
```javascript
const ${1:functionName} = async () => {
  const response = await fetch('${2:URL}');
  const data = await response.json();
  console.log(data);
};$0"
```
#### [fetchez] easy fetch with some options
```javascript
const ${1:functionName} = async () => {
  const response = await fetch('${2:URL}', {
    method: '${3:*GET/POST/PUT/DELETE}',
    headers: {
      'Content-Type': 'application/json',
    },
  });
const data = await response.json();
console.log(data);${0}
};$0"
```
#### [fetchfull] fetch with all options (`*` means default)
```javascript
const ${1:functionName} = async () => {
  const response = await fetch('${2:URL}', {
    method: '${3:*GET/POST/PUT/DELETE}',
    mode: '${4:*same-origin/cors/no-cors}',
    cache: '${5:default*/no-cache/reload/orce-cache/only-if-cached}',
    credentials: '${6:Credentials}',
    headers: {",
      'Content-Type': 'application/json',
      'Accept': 'application/json'
    },
    redirect: '${6:*follow/manual/error}',
    referrer: '${7:*client, no-referrer}',
    body: JSON.stringify(${8:data}),
  });
const data = await response.json();
console.log(data);${0}
};
```
## - Classes -
#### [cla1] simple class (1 prop)
```javascript
class ${1:className} {
  constructor(${2:firstProp}) {
    this.${2:firstProp} = ${2:firstProp};
  }
  $0
}
```
#### [cla2] simple class (add up to 2 props)
```javascript
class ${1:className} {
  constructor(${2:firstProp}, {3:secondProp}) {
    this.${2:firstProp} = ${2:firstProp};
    this.${3:secondProp} = ${3:secondProp};
  }
  $0
}
```
#### [cla3] simple class (add up to 3 props)
```javascript
class ${1:className} {
  constructor(${2:firstProp}, {3:secondProp}, {4:thirdProp}) {
    this.${2:firstProp} = ${2:firstProp};
    this.${3:secondProp} = ${3:secondProp};
    this.${4:thirdProp} = ${4:thirdProp};
  }
  $0
}
```
#### [clex] extended class
```javascript
class ${1:className} extends ${2:parentClass} {
  constructor(${3:parentProps}) {
    super(${3:parentProps});
    ${0}
  }
}
```
#### [con] constructor
```javascript
constructor(${1:params}) {${0}}
```
#### [met] method
```javascript
${1:methodName}(${2:params}) {${0}}
```
#### [pge] propertyGet
```javascript
get ${1:propertyName}() {return this.${0}}
```
#### [pse] propertySet
```javascript
set ${1:propertyName}(${2:value}) {${0}}
```
## - Webpack -
#### [webpack] simple webpack setup
```javascript
const { resolve } = require('path');

const config = {
  entry: ['.${1:./src/index.js}']
  output: {
    path: resolve(__dirname, '${2:dist}'),
    filename: '${3:bundle.js}'
  }$0
};
module.exports = config;
```
#### [modulerules] setup module.rules for loaders
```javascript
module: {
  rules: [
    {
      test: /\.${1:fileExtension}$/,
      use: $0
    }
  ]
}
```
#### [webpackmr] simple webpack setup with module.rules for loaders
```javascript
const { resolve } = require('path');

const config = {
  entry: '${1:./src/index.js}'
  output: {
    path: resolve(__dirname, '${2:dist}'),
    filename: '${3:bundle.js}'
  },
  module: {
    rules: [
      {
        test: /\.${4:fileExtension}$/,
        use: $0
      }
    ]
  }
}

module.exports = config;
```
#### [loader1] A single loader
```json
{
  test: /\.${1:fileExtension}$/,
  use: '$2-loader'
}
```
#### [loader1options] A loader with options 
```json
{
  test: /\\.${1:fileExtension}$/,
  use: {
    loader: '$2-loader',
    options: {
      $0
    }
  }
}$0
```
#### [loader1exc] A loader with exclude
```json
{
  test: /\.${1:fileExtension}$/,
  exclude: ${2:/node_modules/},
  use: '$3-loader'
}
```
#### [loader1inc] A loader with include
```json
{
  test: /\.${1:fileExtension}$/,
  include: __dirname + '${2:dist}', 
  use: '$3-loader'
}
```
#### [loader2] Double loader
```json
{
  test: /\.${1:fileExtension}$/,
  use: ['${2:loader1}', '${3:loader2}']
}
```
#### [loader2exc] Double loader with exclude
```json
{
  test: /\.${1:fileExtension}$/,
  exclude: ${2:/node_modules/},
  use: ['$3-loader', '$4-loader']
}
```
#### [loader2inc] Double loader with include
```json
{
  test: /\.${1:fileExtension}$/,
  include: __dirname + '${2:dist}', 
  use: ['$3-loader', '$4-loader']
}
```
#### [loader3] Triple loader
```json
{
  test: /\.${1:fileExtension}$/,
  use: ['$2-loader', $3-loader, $4-loader]
}
```
#### [loader3exc] Triple loader with exclude
```json
{
  test: /\.${1:fileExtension}$/,
  exclude: ${2:/node_modules/},
  use: ['$3-loader', '$4-loader', '$5-loader']
}
```
#### [loader3inc] Triple loader with include
```json
{
  test: /\.${1:fileExtension}$/,
  include: __dirname + '${2:dist}', 
  use: ['$3-loader', '$4-loader', '$5-loader']
}
```
## - Misc -
#### [dob] destructuring object
```javascript
const {${1:propertyName}} = ${2:objectToDestructFrom}
```
#### [dar] destructuring array
```javascript
const {${1:propertyName}} = ${2:arrayToDestructFrom}
```
#### [stric] use strict
```javascript
'use strict';
```
#### [al] alert
```javascript
alert('${1:msg}');
```
#### [co] confirm
```javascript
confirm('${1:msg}');
```
#### [pm] prompt
```javascript
prompt('${1:msg}');
```
#### [expr] simple express setup
```javascript
const express = require('express')
const app = express();
const port = process.env.PORT || 5000

app.get('/', (req, res) => res.send('Hey there!'));

app.listen(port, () => {
  console.log('Server has started on port ${port}!!!');
});
```
#### [gitbashssh] setup ssh-agent to save your password in your current terminal
```
eval $(ssh-agent -s)
ssh-add ~/.ssh/id_rsa
```
1. Copy and paste these two lines into your terminal
2. Push code to github without re-entering you password

## License
[MIT License]
> The extension can be found on the marketplace @ https://marketplace.visualstudio.com/items?itemName=Cjay.es6-javascript-snippets&ssr=false#overview
