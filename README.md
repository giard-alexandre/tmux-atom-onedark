# Atom OneDark Tmux Theme
> OneDark theme for Tmux. This is basically a copy-paste of the [catpuccin tmux](https://github.com/catppuccin/tmux) theme as I loved the layout of it, but with some color changes to look more like [OneDark Nvim](https://github.com/navarasu/onedark.nvim/blob/master/lua/onedark/palette.lua).

## Themes

- 🌕 [dark](./onedark-dark.tmuxtheme)

## Usage

### TPM

1. Install [TPM](https://github.com/tmux-plugins/tpm)
2. Add the OneDark plugin:

```bash
set -g @plugin 'heuristicAL/tmux-atom-onedark'
# ...alongside
set -g @plugin 'tmux-plugins/tpm'
```

3. (Optional) Set your preferred flavour, it defaults to `"dark"`:
> Currenty, we only have ONE flavor, should change later.

```bash
set -g @onedark_flavour 'dark' # or dark, dark, dark 🙃
```

### Manual

1. Copy your desired theme's configuration contents into your Tmux config (usually stored at `~/.tmux.conf`)
2. Reload Tmux by either restarting the session or reloading it with `tmux source-file ~/.tmux.conf`

#### Configuration options

All flavours support certain levels of customization. To add these customizations, add any of the following options to your Tmux configuration.

In order to have the correct icons displayed please use your favorite nerd fonts patched font.

##### Enable window tabs

By default, the theme places the `window-status` in the `status-right`. With
`@onedark_window_tabs_enabled` set to `on`, the theme will place the
directory within the `status-right` and move the window names to the
`window-status` format variables.

```sh
set -g @onedark_window_tabs_enabled on # or off to disable window_tabs
```

##### Configure separator

By default, the theme will use a round separator for left and right.
To overwrite it use `@onedark_left_separator` and `@onedark_right_separator`

```sh
set -g @onedark_left_separator "█"
set -g @onedark_right_separator "█"
```

##### Enable DateTime

By default, the `date_time` componenet is set to off.
It can be enabled by specifing any tmux date and time format.

```sh
set -g @onedark_date_time "%Y-%m-%d %H:%M"
```

##### Enable User

By default, the `user` componenet is set to off.
It can be enabled by toggoling it on.

```sh
set -g @onedark_user "on"
```

##### Enable Host

By default, the `host` componenet is set to off.
It can be enabled by toggoling it on.

```sh
set -g @onedark_host "on"
```

## 💝 Thanks to

- [Pocco81](https://github.com/catppuccin) and anyone else involved in Catpuccin 😊
