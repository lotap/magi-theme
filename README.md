# Magi Theme

Magi is a palette inspired by [the beautiful UIs of Neon Genesis Evangelion](https://www.reddit.com/r/FUI/comments/762sx3/neon_genesis_evangelion_fui_images_and_gifs/)

<img width="912" alt="Screenshot of lazygit" src="https://github.com/user-attachments/assets/8981ec19-f86a-4c55-a8f4-e3927bab4351">

>To replicate the exact look of this screenshot, you will need:
>
> - MesloLG [Nerd Font](https://github.com/ryanoasis/nerd-fonts)
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
> git:
>   paging:
>     pager: "delta --paging=never"
> ```

## Palette

<details>
<summary>Color swatches</summary>

![Color Picker - F06800](https://github.com/user-attachments/assets/103854fb-f976-4cfc-acf1-3a152155f01f)

![magi-normal](https://github.com/user-attachments/assets/921d002d-d7fa-4bc0-8809-1783b89c9268)

![magi-bright](https://github.com/user-attachments/assets/9bdc9a91-1106-4623-b0f7-434fae052896)
</details>

Orange Primary: #f06800

| Color   | Normal  | Bright  |
| ------- | ------- | ------- |
| Black   | #000000 | #484848 |
| Blue    | #5090c8 | #40c8e8 |
| Cyan    | #60f0a0 | #3cffd0 |
| Green   | #409820 | #50ff10 |
| Magenta | #7058a4 | #b040a0 |
| Red     | #a00010 | #c80010 |
| White   | #b0b0b0 | #f8f8f8 |
| Yellow  | #f0f0a0 | #f4b000 |

## Usage

> ~~So far, I have only made this into an [Alacritty](https://github.com/alacritty/alacritty) theme, but more may come.~~

### Alacritty

Copy the contents of `alacritty.toml` into your alacritty config file (`~/.config/alacritty/alacritty.toml` by default)

Or download the whole file and import it:

```toml
[general]
import = ["~/.config/alacritty/themes/magi.toml"]
```

### Ghostty

> I don't have beta access, so the current config is my best guess based on what's in <https://github.com/mbadolato/iTerm2-Color-Schemes/tree/master/ghostty>

Copy the contents of `ghostty` and paste the content in your [Ghostty](https://github.com/ghostty-org) config file (`~/.config/ghostty/config`)
