# lua-import

Library for importing dependencies with a more terse syntax

## Import usage

On top of your file:

```lua
local Layer, Graphics, Data; import()
```

This code is equivalent to:
```lua
local Layer = require('Layer')
local Graphics = require('Graphics')
local Data = require('Data')
```

Additionally, you can also provide a path on the import, so it will be used in all the requires:

```lua
local Layer, Graphics, Data; import('lib/')
```

Does same as:

```lua
local Layer = require('lib/Layer')
local Graphics = require('lib/Graphics')
local Data = require('lib/Data')
```
