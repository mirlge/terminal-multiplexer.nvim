# [Actual repo](https://codeberg.org/mirge/terminal-multiplexer.nvim)

# terminal-multiplexer.nvim

## Not maintained anymore

This plugin is no longer maintained, because it's not necessary. tmux is enough.

## Installation

### Using [💤 lazy.nvim](https://github.com/folke/lazy.nvim)

```lua
{
  "mirlge/terminal-multiplexer.nvim",
  url = "https://codeberg.org/mirge/terminal-multiplexer.nvim",
  opts = {
    -- config goes here
  },
}
```

## Setup (if necessary)

```lua
require("terminal-multiplexer").setup({
  -- config goes here
})
```

## Default config

```lua
{
  prefix = "<C-s>",
  detach_keymap_func = , -- keymap function, see `defaults.lua` for the default
}
```

## Keymaps

* `<prefix>d`: Detach from current session
* `<prefix>[np]`: Go to next/previous tab
* `<prefix>c`: Create a new tab with a terminal
* `<prefix>%`: Split vertically with a terminal
* `<prefix>"`: Split horizontally with a terminal
* `<prefix>$`: Rename current session
* `<prefix><Esc>`: Get out of terminal mode

> [!NOTE]
> if you are in terminal mode and press the key after the prefix key too slow,
> and therefore freeze your terminal, you can unfreeze your terminal with `<C-q>`
> (at least in bash and zsh)
