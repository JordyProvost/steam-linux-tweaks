Game does not start

Execute this command :

```echo SDL_VIDEO_X11_VISUALID=$(glxinfo | grep -A 1000 "GLX Visuals" | grep None | tail -n1 |awk -F' ' '{print $1}') %command%```

Copy the output and paste it in the "Launch options" field of the steam game properties
