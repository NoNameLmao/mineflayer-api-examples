# bot.world

A synchronous representation of the world. Uses [prismarine-world](https://github.com/PrismarineJS/prismarine-world).

## Events

### **"blockUpdate" (oldBlock, newBlock)**

Fires when a block updates.
Both old and new blocks are provided for comparison.

⚠️ **oldBlock** may be `null`

### **"blockUpdate:(x, y, z)" (oldBlock, newBlock)**

Fires only when a block at a specific coordinate is changed.
Also provides both old and new blocks.

⚠️ **oldBlock** may be `null`
