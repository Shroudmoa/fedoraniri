# Installing Niri and DMS

### Step 1: Enable the COPR Repository

```bash
sudo dnf copr enable avengemedia/dms
```
### Step 2: Install Niri and DMS
```bash
sudo dnf install niri dms
```
### Step 3: Enable DMS for the Niri session
```bash
systemctl --user add-wants niri.service dms
```
# Starting Niri
> Log out and log in using the Niri session.
&nbsp;

# Session Cleanup

### Kill waybar
```bash
pkill -f waybar
```

### Kill quickshell
```bash
pkill -f quickshell
```

### Kill Dankbar
```bash
pkill -f dankbar
```

### Kill GNOME Shell
```bash
pkill -f gnome-shell
```
> Warning: Killing gnome-shell will immediately close the GNOME desktop session.
# Configuration File Paths

### 1. Niri Configuration
Copy the provided config.kdl file into:

`~/.config/niri/config.kdl`

---
### 2. Custom Application Launcher (Optional)

Fuzzel Config File :
```bash
mkdir -p ~/.config/fuzzel

nano ~/.config/fuzzel/fuzzel.ini
```