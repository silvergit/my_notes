# Deltup

Install `xdelta3` from the official repositories. 

Edit `/etc/pacman.d/mirrorlist` and add the proper repository:

`/etc/pacman.d/mirrorlist`
```
##
## Arch Linux repository mirrorlist
## Generated on 2011-03-24
##

## Delta Archlinux.fr
Server = http://delta.archlinux.fr/$repo/os/$arch
.....
```
Then edit `/etc/pacman.conf` uncommenting (removing #) the option UseDelta:

`/etc/pacman.conf`
```
.....
# Misc options (all disabled by default)
#UseSyslog
ShowSize
UseDelta
TotalDownload
.....
```
