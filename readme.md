This is a test example demonstrating an issue with npm where as it cannot install a package using a local file module.  
This package can be examined in detail at [here](https://github.com/tabersays/tabersays-this-is-a-test)  
`npm i tabersays-this-is-a-test` give the error:
```javascript
npm ERR! code ENOLOCAL
npm ERR! Could not install from "node_modules/tabersays-this-is-a-test/lib/some" as it does not contain a package.json file.

```
package.json
```javascript
...
"dependencies": {
    "some": "file:./lib/some"
  }
...
```