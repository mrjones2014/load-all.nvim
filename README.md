# load-all.nvim

Allows you to load all Lua files in a directory at once. Note, this uses `dofile`, not `require`, so it doesn't
return anything, it just executes the Lua files via `dofile`.

## Requirements

Neovim >0.5.0

## Installation

### Packer

```lua
use { 'mrjones2014/load-all.nvim', requires = 'nvim-lua/plenary.nvim' }
```

### Vim Plug

```VimL
Plug 'nvim-lua/plenary.nvim'
Plug 'mrjones2014/load-all.nvim'
```

## Usage

```lua
require('load-all')(path)
-- for example
require('load-all')(os.getenv('HOME') .. '/.config/nvim/lua/plugins')
```
