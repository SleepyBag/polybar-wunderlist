# polybar-wunderlist
Wunderlist module for polybar.

# Dependencies
* zsh (located at /bin/zsh, or you will need to modify the path of zsh in the scripts)
* inotifywait
* [wunderline](https://github.com/wayneashleyberry/wunderline)

# Installation
Put all of these files into a standalone directory. And then write into polybar config:

```
[module/wunderlist]
type = custom/script

exec = /path/to/wunderlist/monitor
tail = true
scroll-up = "/path/to/wunderlist/index_down"
scroll-down = "/path/to/wunderlist/index_up"
```

# Usage
Initially, run **./wunderlist** at background, it will update the content file every several tens of seconds.
Then you are easy to go, add the modul into your bar and it will show a list of your undo items. Scroll on the module to select which item to expand.
