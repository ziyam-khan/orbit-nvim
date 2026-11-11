<h1 align="center">orbit-nvim</h1>
<p align="center">My user configuration for AstroNvim v3: a dark dashboard, format on save, and language tooling through Mason.</p>

<p align="center">
  <img alt="Neovim" src="https://img.shields.io/badge/Neovim-0.8%2B-57a143">
  <img alt="AstroNvim" src="https://img.shields.io/badge/AstroNvim-v3-0f1b2e">
  <img alt="Lua" src="https://img.shields.io/badge/config-Lua-000080">
</p>

## What is in it

- **Look:** the `astrodark` colourscheme, a pure-black background override for `duskfox`, and an ASTRO NVIM banner on the dashboard.
- **Editing:** format on save for every language server that can format, with a one-second timeout; diagnostics as virtual text.
- **Tooling:** Mason installs the language servers, formatters and debug adapters; null-ls wires the formatters; Treesitter handles highlighting.
- **Room to grow:** AstroCommunity is loaded, so a plugin pack is one `import` line in `plugins/community.lua`.

It started from AstroNvim's user template, and it targets AstroNvim v3. AstroNvim v4 and later read their configuration differently.

## Install

Back up what you have, then clone AstroNvim v3 and this configuration as its `user` folder:

```sh
mv ~/.config/nvim ~/.config/nvim.bak
mv ~/.local/share/nvim ~/.local/share/nvim.bak

git clone --depth 1 --branch v3.45.3 https://github.com/AstroNvim/AstroNvim ~/.config/nvim
git clone https://github.com/ziyam-khan/orbit-nvim ~/.config/nvim/lua/user
nvim
```

The first start installs every plugin.

## Layout

| File | What it sets |
|---|---|
| `init.lua` | Updates, colourscheme, diagnostics, LSP formatting |
| `options.lua`, `mappings.lua` | Vim options and key mappings |
| `plugins/` | Dashboard, Mason, none-ls, Treesitter, AstroCommunity and your own plugins |
| `highlights/` | Highlight overrides per colourscheme |

---

By [Ziyam Khan](https://ziyamkhan.com) · [GitHub](https://github.com/ziyam-khan)
