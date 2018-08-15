## drop-console-webpack-plugin
#### A webpack plugin for removing console and supporting webpack4
![](https://img.shields.io/badge/npm-1.1.5-blue.svg)
![](https://img.shields.io/badge/build-passing-brightgreen.svg)
![](https://img.shields.io/badge/license-MIT-brightgreen.svg)
## Installation
```
npm install drop-console-webpack-plugin --save
```
## Usage
```
    const DropConsoleWebpackPlugin = require('drop-console-webpack-plugin')

    plugins: [
        new DropConsoleWebpackPlugin(),
    ]
```
## Notes
```
if   webpack version < 4    :    2.0>drop-console-webpack-plugin version >1.2    
if   webpack version >= 4   :    drop-console-webpack-plugin version >2.0 && nodejs version > 7.6
```
## Options
```
Name | type | default | Description
---- | ---- | ------- | -----------
drop_log | Boolean | true | remove console.log(...)
drop_info | Boolean | true | remove console.info(...)
drop_warn | Boolean | true | remove console.warn(...)
drop_error | Boolean | true | remove console.error(...)
```
## Code
```
new DropConsoleWebpackPlugin({
    drop_log    : true, 
    drop_info   : true,
    drop_warn   : true,
    drop_error  : true,
})
```