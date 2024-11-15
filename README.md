# sway-obs
 things to test for sway and obs

install sddm

/usr/share/wayland-sessions/sway.desktop
[Desktop Entry]
Name=Sway
Comment=An i3-compatible Wayland compositor
Exec=env XDG_CURRENT_DESKTOP=sway dbus-run-session sway
Type=Application

/etc/portage/make.conf
USE="pulseaudio pipewire wayland screencast gstreamer gles2"

/etc/portage/package.use/obs
media-video/obs-studio pipewire
media-video/pipewire dbus

install qtwebkit

~/.config/sway/config
exec --no-startup-id dbus-update-activation-environment --all
exec gentoo-pipewire-launcher restart &

waybar

set $menu bemenu-run -H 26--no-exec -p  "" | xargs swaymsg exec --

