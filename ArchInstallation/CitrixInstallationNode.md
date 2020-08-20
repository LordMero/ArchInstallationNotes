# Notes on how to install Citrix Workspace on Arch 

* Follow the instructions here as root! 
https://docs.citrix.com/en-us/citrix-workspace-app-for-linux/install.html

* set up the correct env variable ICAROOT

* Create a .desktop file in .locale/share/applications/citrix.desktp

[Desktop Entry]
Name=ICA handles
Comment=use wfica to open ica files from citrix
Exec=/opt/Citrix/ICAClient/wfica %f
Icon=""
Terminal=false
Type=Application
Categories=Editor;
StartupNotify=true
MimeType=application/x-wine-extension-ini;

* Associate citrix.desktop to the filetype by  runnig 
xdg-mime default citrix.desktop application/x-wine-extension-ini




