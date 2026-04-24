# Magi Theme

Magi is a palette inspired by [the beautiful UIs of Neon Genesis Evangelion](https://www.reddit.com/r/FUI/comments/762sx3/neon_genesis_evangelion_fui_images_and_gifs/)

<img width="912" alt="Screenshot of lazygit" src="https://github.com/user-attachments/assets/3d5936f1-9ee8-41e4-b63e-f457c5435b6c">

> To replicate the exact look of this screenshot, you will need:
>
> - [Commit Mono](https://commitmono.com/) [Nerd Font](https://github.com/ryanoasis/nerd-fonts)
> - [Delta](https://github.com/dandavison/delta)
> - [Lazygit](https://github.com/jesseduffield/lazygit)
>
> Delta Config (`~/.gitconfig`)
>
> ```ini
> [core]
>   pager = delta
>
> [delta]
>   line-numbers = true
>   syntax-theme = base16 # This theme only uses colors set by the terminal
> ```
>
> [Lazygit Config](https://github.com/jesseduffield/lazygit/blob/master/docs/Config.md) (`.lazygit.yml` in your repo parent dir)
>
> ```yaml
> gui:
>   nerdFontsVersion: "3"
>   showFileIcons: true
>   theme:
>     selectedLineBgColor:
>       - bold
> git:
>   paging:
>     pager: "delta --paging=never"
> ```

## Palette

<details>
<summary>Color swatches</summary>

> [!WARNING]
> These swatches are out-of-date with the current colors. Refer to the table below for updated hex codes. I will update the swatches once I'm confident that each color has settled on a final value. The current swatches should still provide a good idea of the overall palette, the tweaks are for better visual contrast in a terminal or for more alignment with the colors in the show.

![Color Picker - F06800](https://github.com/user-attachments/assets/103854fb-f976-4cfc-acf1-3a152155f01f)

![magi-normal](https://github.com/user-attachments/assets/921d002d-d7fa-4bc0-8809-1783b89c9268)

![magi-bright](https://github.com/user-attachments/assets/9bdc9a91-1106-4623-b0f7-434fae052896)

</details>

Orange Primary: #ec7420

| Color   | Normal  | Bright  |
| ------- | ------- | ------- |
| Black   | #000000 | #484848 |
| Red     | #a80808 | #f02020 |
| Green   | #409820 | #50ff10 |
| Yellow  | #f4b000 | #f0f0a0 |
| Blue    | #5090c8 | #40c8e8 |
| Magenta | #a06090 | #b040a0 |
| Cyan    | #60f0a0 | #3cffd0 |
| White   | #b0b0b0 | #e8e8e8 |

## Usage

### Alacritty

Copy the contents of `alacritty.toml` into your alacritty config file (`~/.config/alacritty/alacritty.toml` by default)

Or download the whole file and import it:

```toml
[general]
import = ["~/.config/alacritty/themes/magi.toml"]
```

### Ghostty

Copy the contents of `ghostty.conf` and paste the content in your [Ghostty](https://github.com/ghostty-org) config file (`~/.config/ghostty/config`)

### Fish Shell

Copy the contents of `fish-magi.theme` or `fish-eva.theme` to `~/.config/fish/themes/magi.theme` then run `fish_config theme save magi`

The magi theme uses cyan & yellow for commands whereas the eva theme uses green & magenta.

If the theme is not saving between sessions, the automatically generated `fish_frozen_theme.fish` is probably not updating. Try using the `fish_config` command, selecting `magi` from the ui and clicking the `set theme` button.

#### [Tide](https://github.com/IlanCosman/tide)

Add to your fish config file `~/.config/fish/config.fish`:

```fish
set -g tide_character_color yellow
set -g tide_git_color_branch yellow
set -g tide_pwd_color_anchors brwhite
set -g tide_pwd_color_dirs white
```

#### [Starship](https://starship.rs/)

Add to your Starship config file `~/.config/starship.toml`:

```toml
"$schema" = 'https://starship.rs/config-schema.json'

[directory]
style = "white bold"

[git_branch]
style = "bold yellow"

[character]
success_symbol = "[❯](bold yellow)"

```
