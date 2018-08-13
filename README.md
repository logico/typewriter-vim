# Typewriter [▎](https://logico.com.ar)

  A minimalistic vim and gvim colorscheme inspired by the great iA Writer editor.
  This repo contains the light (typewriter.vim) and dark (typewriter-dark.vim)
  versions.

## Installation

  - You can use your vim plugin manager of choice
  - Or manually
    - Clone this repo.
    - Copy `colors/*.vim` to `~/.vim/colors/`


## Usage

  To enable this colorscheme, set in your .vimrc file:

  ```vim
    colorscheme typewriter
    " or typewriter-night
  ```

## Extras

  If you want a closer feel to iA Writer install

  - [goyo.vim](https://github.com/junegunn/goyo.vim) for focus mode.
  - [limelight.vim](https://github.com/junegunn/limelight.vim) for line
    highlight.

  and add this lines to vimrc:

  ```vim
    " Activate FOCUS mode with F12
    nmap <F12> :Goyo <bar> Limelight!!<CR>"


    " Change the cursor from block to i-beam in INSERT mode
    let &t_SI = "\e[5 q"
    let &t_EI = "\e[1 q"
    augroup myCmds
      au!
      autocmd VimEnter * silent !echo -ne "\e[1 q"
    augroup END
  ```

### Screenshots

![vim](https://logico.com.ar/img/2018/08/13/screenshot_a.png)

  ![gui vim](https://logico.com.ar/img/2018/08/13/screenshot_g.png)

  ![vim focus mode](https://logico.com.ar/img/2018/08/13/screenshot_b.png)

  ![fake bussy](https://logico.com.ar/img/2018/08/13/screenshot_c.png)

  ![typewriter night vim](https://logico.com.ar/img/2018/08/13/screenshot_d.png)

  ![typewriter night vim focus mode](https://logico.com.ar/img/2018/08/13/screenshot_e.png)

  ![typewriter night gui vim](https://logico.com.ar/img/2018/08/13/screenshot_f.png)

  The font used in the screenshots is SF Mono 12 with letter space of -1 and
  line space of 8.

  ```
    # .Xresources file
    URxvt*letterSpace   : -1
    URxvt*lineSpace     : 8
  ```

  or if you use gVim o MacVim

  ```
    # .gvimrc file
    set linespace = 8
  ```

---

## Thanks

  Typewriter is based/inspired by these projects

  - [iA Writer](https://ia.net/writer/)
  - [Vim colorschemes](https://github.com/flazz/vim-colorschemes)

