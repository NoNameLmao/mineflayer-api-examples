# blocks

A map of all blocks that exist in a version,
indexed by their ids.

`[ '0': {}, '1': {}, '2': {}, ... ]`
```js
const mcdata = require('minecraft-data')('1.12.2');
console.log(mcdata.blocks['0'])
/*
{
    id: 0,
    displayName: 'Air',
    name: 'air',
    hardness: 0,
    stackSize: 0,
    diggable: true,
    boundingBox: 'empty',
    drops: [ { drop: 0 } ],
    transparent: true,
    emitLight: 0,
    filterLight: 0,
    resistance: 0,
    minStateId: 0,
    maxStateId: 15,
    defaultState: 0
}
*/
