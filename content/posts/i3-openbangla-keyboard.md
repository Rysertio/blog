---
title: "Configuring Openbangla Keyboard for i3"
date: 2022-11-25T16:43:34+06:00
draft: true
---
# Configuring Openbangla Keyboard for i3
In order to configure openbangla keyboard for i3 you need to add these lines to your `/etc/environment`. So the configuration would persist even if you've changed your shell.
```
GTK_IM_MODULE=ibus
QT_IM_MODULE=ibus
XMODIFIERS=@im=ibus
```

Then add this line to your i3 config file (`~/.config/i3/config` by default) in order start ibus automatically whenever you start i3.  
`exec ibus-daemon -drxR`

