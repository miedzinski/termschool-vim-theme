# termschool
## An improved codeschool like vim theme for 256-color terminals

termschool is a vim theme optimized for 256-color terminals. The theme "medium/dark" and makes heavy use of greys, greens and blues in pastel tones. You can [preview termschool here](http://vimcolors.com/375/termschool/dark).

The original codeschool for 256-color terminals was created by @Astonj (http://astonj.com) based on the
editor used at http://codeschool.com. While I enjoyed the theme, I felt it could use a number of
improvements and started implementing them for private use. At some point, my version started to differ
from the original and I decided to release it for public use, with the name "termschool" (think "Codeschool
for terminals.")

Keep in mind that this theme is a constant work in progress. I use editors all day and once in a while I'll
stumble on some color combination that I don't quite like. When that happens, I'll update the theme and
push a change. Fork this repository if you prefer a theme that will never change, or keep pulling newer
versions if you like my fixes and improvements.

# Installation

## Using Vundle

If you're using Vundle, just add the following to your `~/.vimrc` file:

```VimL
Plugin 'marcopaganini/termschool-vim-theme'
colorscheme termschool
```

While still inside vim, type: `<ESC>:PluginInstall`. This should install termschool automatically. Restart vim and the new theme should be the default.

## Manual installation

Manual installation is very simple: Download the `termschool.vim` file and copy it into your `~/.vim/colors` directory. Edit your `~/.vimrc` file and add:

```VimL
colorscheme termschool
```
Restart vim and everything should work.

A better (but slightly more complicated) option is to git clone this repository somewhere in your disk and create a symlink from the `termschool.vim` file inside your working repository to `~/.vim/colors`.

## Caveats

Please note that this theme *requires* a 256-color capable terminal. Most popular terminals are 256-color capable these days, but if things look odd, your terminal might not have this capability.

If you know your terminal is 256-color capable and things still look ugly/weird, try adding the following to
your `~/.vimrc` file right before the `colorscheme termschool` line:

```VimL
set t_Co=256                                                                                        
```

This will force vim to use 256 colors.

Note that the theme has been tuned for 256-color terminals (I just can't match the productivity of screen + vim on gvim) but should also work fine for GUI environments.

Feel free to send comments with ideas, suggestions and push requests.
