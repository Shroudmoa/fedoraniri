# To install Niri


sudo dnf copr enable avengemedia/dms


sudo dnf install niri dms


systemctl --user add-wants niri.service dms


#################################################
#Logout and Login with niri 
#kill the tasks that we dont need anymore


pkill -f waybar


pkill -f quickshell


pkill -f dankbar


pkill -f gnome-shell


# NIRI Config File :


~/.config/niri/config.kdl

# Fuzzel Config File :
#mkdir -p ~/.config/fuzzel

#nano ~/.config/fuzzel/fuzzel.ini
