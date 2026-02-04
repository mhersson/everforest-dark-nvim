# Everforest Dark for Neovim

A Neovim colorscheme based on the
[Everforest](https://github.com/sainnhe/everforest) dark medium palette, ported
from the Helix editor theme.

## Installation

### lazy.nvim

```lua
{
    "mhersson/everforest-dark-nvim",
    lazy = false,
    priority = 1000,
    config = function()
        require("everforest").setup()
        vim.cmd.colorscheme("everforest")
    end,
}
```

### Local development

```lua
{
    dir = "~/path/to/everforest-dark-nvim",
    lazy = false,
    priority = 1000,
    config = function()
        require("everforest").setup()
        vim.cmd.colorscheme("everforest")
    end,
}
```

## Supported Plugins

- **Completion**: blink.cmp, nvim-cmp
- **Diagnostics**: Built-in LSP diagnostics
- **File Navigation**: snacks.nvim (picker, notifier, dashboard, indent)
- **Git**: gitsigns.nvim, neogit
- **Testing**: neotest
- **Debugging**: nvim-dap-ui
- **UI**: noice.nvim, which-key.nvim, trouble.nvim, flash.nvim
- **AI**: Copilot (native LSP inline completion)
- **Misc**: mini.nvim (indentscope)

## Color Palette

| Color  | Hex       | Usage                        |
| ------ | --------- | ---------------------------- |
| bg_dim | `#232a2e` | Dimmed background            |
| bg0    | `#2d353b` | Default background           |
| bg1    | `#343f44` | Cursor line, folded          |
| bg2    | `#3d484d` | Floating windows             |
| bg3    | `#475258` | Visual selection, statusline |
| bg4    | `#4f585e` | Window separators            |
| fg     | `#d3c6aa` | Default foreground           |
| red    | `#e67e80` | Keywords, errors             |
| orange | `#e69875` | Operators, labels            |
| yellow | `#dbbc7f` | Types, warnings              |
| green  | `#a7c080` | Functions, strings           |
| aqua   | `#83c092` | Strings, special             |
| blue   | `#7fbbb3` | Properties, info             |
| purple | `#d699b6` | Constants, hints             |
| grey0  | `#7a8478` | Line numbers, inactive       |
| grey1  | `#859289` | Comments, borders            |
| grey2  | `#9da9a0` | Cursor line number           |

## Credits

- Original Everforest theme by [sainnhe](https://github.com/sainnhe/everforest)
- Helix port by CptPotato and basbebe

## License

MIT License
