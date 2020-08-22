<p align="center">
  <img width="25%" src="https://github.com/Sam1431/Gentoo-BSPWM/blob/master/gentoo.png" />
</p>

<p align="center">
  <b> Sam's BSPWM setup </b>
</p>

<img src="https://github.com/Sam1431/Gentoo-BSPWM/blob/master/Gentoo.png" alt="img" align="right" width="400px">

This is my BSPWM setup

The [setup section](#setup) will guide you through the installation process.

****

## My Specs:

+ **WM**: [BSPWM](https://github.com/baskerville/bspwm)
+ **OS**: Gentoo
+ **Shell**: [Fish](https://fishshell.com/)
+ **Terminal**: [Alacritty](https://github.com/alacritty/alacritty)
+ **Org editor**: [Doom Emacs](https://github.com/hlissner/doom-emacs/)
+ **File Manager**: [Thunar](https://git.xfce.org/xfce/thunar/)
+ **Launcher**: [Dmenu](https://tools.suckless.org/dmenu/)
+ **Browser**: Firefox

****

## New stuff

- Code Name : GALAHAD 
- Now much more Keyboard centric
- Retro Theme [ INSTEAD OF MINIMALISM ]

****

## Setup

Here are the instructions you should follow to replicate my BSPWM setup.
> 1. Dependencies
  
  You will need the following packages
  
  + **BspWM** - Obviously
  + **SXHKD** - Simple X HotKey Daemon [ FOR THE KEYBINDINGS ]
  + **Polybar** - Status Bar
  + **Alacritty** - Terminal used
  + **Dmenu2** - can be found in the repo's needed dependencies file [ Main Menu ]
  + **KsuperKey** - For some keybindings to work [ also will be found the needed dependencies file ]
  
****  
  
> 2. Install needed fonts

   You will need to install a few fonts (mainly icon fonts) in order for text and icons to be rendered properly.

   Necessary fonts:
   
   + **FontAwesome** - [ dependency for polybar ]
   + **Icomoon-feather** - [ can be found in ~/home/.config/polybar/fonts]
   + **Ubuntu-Condensed** - [ can be found in ~/.home/.config/polybar/fonts ]
   + **Any one nerd font** - [website](https://www.nerdfonts.com/font-downloads)
>
>   
   - paste the .ttf fonts to `~/.local/share/fonts`.
   - It does not matter that the actual font files (`.ttf`) are deep inside multiple directories. They will be detected as long as they can be accessed from `~/.fonts` or `~/.local/share/fonts`.

   Finally, run the following in order for your system to detect the newly installed fonts.
   ``` in your terminal
   fc-cache -v
   ```
****   
> 3. Install my BSPWM configuration files

   ``` in your terminal 
   git clone https://github.com/Sam1431/Gentoo-BSPWM.git
   ```
>
>
****
> 4. Placement 
  
   ```
   Files in /Gentoo-BSPWM/.bin ----> /bin
   Files in /Gentoo-BSPWM/.config ----> ~/home/.config
   .mpd ----> ~/home [optional]
   .ncmpcpp ----> ~home [optional]
   compile the files in needed dependencies [ KsuperKey & Dmenu2 ]
   ```
   
****
   
## Keybinds

I use <kbd>super</kbd> as my modkey

#### Keyboard
| Keybind | Action |
| --- | --- |
| <kbd>super + enter</kbd> | Spawn terminal |
| <kbd>super</kbd> | Launch dmenu (Super + d , if ksuperkey is not installed) |
| <kbd>super + x</kbd> | Close client |
| <kbd>super + space</kbd> | Toggle floating client |
| <kbd>super + [1-0]</kbd> | change workspace |
| <kbd>super + shift + [1-0]</kbd> | Move focused client to tag |
| <kbd>super + w</kbd> | Tiling layout |
| <kbd>super + space</kbd> | Floating layout |
| <kbd>super + f</kbd> | Maximized / Monocle layout |
| <kbd>super + [arrow keys]</kbd> | Change focus by direction |
| <kbd>super + shift + [arrow keys]</kbd> | Move client by direction. |
| <kbd>super + alt + [arrow keys]</kbd> | expand client in the given direction |
| <kbd>super + control + [arrow keys]</kbd> | shrink client in the given direction |
| <kbd>super + f</kbd> | Toggle fullscreen |

*... And many many more.*

****

#### Mouse
| Mousebind | Action |
| --- | --- |
| `Super + right mouse button(drag)` | Resize Client (In floating) |
| `Super + Left Mouse Button (drag)` | Move Client (In floating) |

****

 > Don't forget to star this repo [ just for fun ] 💙
