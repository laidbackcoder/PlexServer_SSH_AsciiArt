# Plex Media Server - Ascii Art
Plex Logo Ascii Art Example:

![Plex Logo in ASCII Art](https://github.com/laidbackcoder/PlexServer_SSH_AsciiArt/blob/main/Screenshots/Plex%20Logo%20Ascii%20Art%20Example.png)

# Show on SSH Connection

To display the ASCII Art when a user connects to a Linux server via SSH, add the following text to the end of the `"/etc/bash.bashrc"` file on the server:


```Shell
if [[ -n $SSH_CONNECTION ]] ; then

    clear
    
    echo "Welcome to..."
    echo ""
    echo -e " ██████  ██      ███████ \e[93m██\e[39m   ██ "
    echo -e " ██   ██ ██      ██       \e[93m██\e[39m ██  "
    echo -e " ██████  ██      █████     \e[93m███\e[39m   "
    echo -e " ██      ██      ██       \e[93m██\e[39m ██  "
    echo -e " ██      ███████ ███████ \e[93m██\e[39m   ██ "
    echo -e "                    \e[1mMedia Server"
    echo ""

fi
```

On connection, it will look something like this:

![Plex Logo in ASCII Art - SSH Example](https://github.com/laidbackcoder/PlexServer_SSH_AsciiArt/blob/main/Screenshots/Initial%20SSH%20Connection%20Example.png)
