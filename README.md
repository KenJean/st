# An Expert Noob build of ST - The suckless/simple terminal
> for arch users
- Literally the best terminal i have ever used having an awesome unicode(🤣🙂😈👋) support.
- Minimalist free from bloat.
- From suckless

## This build provide out of the box support for
- **Emoji and special character.** (Yeah man emoji in terminal💀👹👽 it's really cool)
- **Transparency.**
- **Scrollback.**
- **Cursor Blinking.**
- **Gruvbox Color Scheme.** (A color scheme which just feels light on eyes)

YKH: ligatures for Fira Code

## screenshots
![st1](https://user-images.githubusercontent.com/70854893/92417516-42f9da80-f180-11ea-9609-53ffecd0ded4.png)


## Steps before installation.
- Replace libxft package with libxft-bgra for BGRA glyphs and scaling support(emoji).
  You can install libxft-bgra-git from aur using aur helper
  or you can also make it on your own.
  Emoji rendering is not the problem of st it's because of libxft.
  For more details [libxft-bgra](https://gitlab.freedesktop.org/xorg/lib/libxft/-/merge_requests/1)
``````
yay -S libxft-bgra-git
``````
- Install fonts for emoji support.
``````
sudo pacman -S ttf-joypixels
``````
> or you can also install any other emoji font.

## Installation

- Clone the repo and install it.
````
git clone https://github.com/google-was-my-idea/st.git
cd st
sudo make install
````
## Key bindings
- scroll up and down using shift+j and shift+k.
- zoom out and zoom in using ctrl+shift+up and ctrl+shift+down.
- ctrl+shift+left for zoomreset.
- ctrl+shift+c and ctrl+shift+v for copy and paste.
- You can also bind your own keys by changing config.h file.

## Details of the patches applied
- alpha
- blinking cursor
- desktopentry
- gruvbox
- font2
- scrollback

## You can also build your own st
> check out more patches at [suckless](https://st.suckless.org/)

## More gruvbox color scheme
> [gruvbox](https://github.com/morhetz/gruvbox)

Thanks and Enjoy this build !
