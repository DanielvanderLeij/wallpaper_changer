# wallpaper_changer
A wallpaper changer for Gnome desktops.
This script assumes that there is a /wallpapers directory in the home directory.
All .jpeg files in the /wallpapers folder will be taken and randomly set as wallpaper every hour.
If you have different image formats, copy the code on line 7 and paste it below line 7 and change '.jpeg' to the file format you need.

To make this script start on system startup, place these lines at the bottom of the .profile file in your home folder:
# start my custom script for setting random background wallpapers
if [ -f "$HOME/.change_wallpaper" ] ; then
    bash $HOME/.change_wallpaper &
fi
