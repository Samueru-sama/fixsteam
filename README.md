# Notice

I've moved to using this Steam AppImage which contains several of the fixes of this script + it also contains the EAC-Gblic patch.

https://github.com/Samueru-sama/Steam-appimage

By making a directory next to the AppImage with then name of the AppImage + `.home` you also get rid of the useless dotfiles that Steam puts in $HOME.

----------------------------------------------------------------------

# fixsteam
This script fixes multiple issues that the linux version of Steam has.

Fixes these issues: 

https://github.com/ValveSoftware/steam-for-linux/issues/5607

https://github.com/ValveSoftware/steam-for-linux/issues/1890

Also launches Steam silently (doesn't steal focus) by default. 

# USAGE

* Place the script in `$HOME/.local/bin`
* Make sure `$HOME/.local/bin` is first in `$PATH`. Do a `echo $PATH` to confirm that. 
* Lauch the script once thru the terminal, as it will copy and patch the `steam.desktop` to `$XDG_DATA_HOME/applications` so that the script is called every time Steam is launched by its .desktop file.

If you don't have `$HOME/.local/bin` in your PATH and/or it is not FIRST in PATH, add this to your `.bash_profile` or `.zprofile`:

```
export PATH="$HOME/.local/bin:$PATH"
```

# READ THIS

If you get `LD_PRELOAD cannot be preloaded (cannot open shared object file)` errors when launching the script from the terminal, that is normal and everything should still work like it should. See [here](https://github.com/Samueru-sama/fixsteam/issues/1)

----------------------------------------------------

Credit and big thanks goes to https://github.com/RunningDroid for the screensaver fix: 
https://gitlab.com/RunningDroid/misc-scripts/-/blob/master/steam?ref_type=heads





   


