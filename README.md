# Forked-kakoune-easymotion
​
[kakoune](http://kakoune.org) plugin for navigating like the easymotion vim mode

__NB : This forked made some modifications to be compatible with newer versions of Kakoune and fixed some issues. Moreover, it's modified mainly to suits my own needs and to make it permanant.__

![demo](https://github.com/danr/kakoune-easymotion/blob/master/recording.gif?raw=true)

## Setup

Add `easymotion.kak` to your autoload directory,`~/.config/kak/autoload`, or source it manually. __In my config `kakrc`, it looks like this :__

```
plug "https://github.com/alexblanc1/kakoune-easymotion-alex.git" config %{
    face global EasyMotionBackground rgb:000001
    face global EasyMotionForeground rgb:ee3a8c,rgb:000000+fg
    face global EasyMotionSelected yellow+b
    # new map bidirectionnal
    map global easymotion e ': easy-motion-word<ret>' -docstring 'word ↔'
    map global easymotion l ': easy-motion-line<ret>' -docstring 'line ↔'
    map global easymotion c ': easy-motion-char<ret>' -docstring 'char ↔'
}
# --- Entrer easymotion mode ---
map global normal <a-space> ': enter-user-mode easymotion<ret>'
```






## License

Unlicense
