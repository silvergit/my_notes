install `bicon`

run `bicon`

OR

su
echo 'Terminal=true' >> /usr/share/applications/xfce4-terminal.desktop
echo 'Exec=/usr/bin/bicon' >> /usr/share/applications/xfce4-terminal.desktop


gconftool-2 --set --type=string /apps/gnome-terminal/profiles/Default/encoding en_US.UTF-8

