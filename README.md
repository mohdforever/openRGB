# openRGB
NOT official repo for openRGB plugin and udev


Visit official website at https://openrgb.org

################################################################################


Installing UDEV rules manually

If you have installed OpenRGB from a package then latest UDEV rules are installed locally at /usr/lib/udev/rules.d/60-openrgb.rules
Flatpak and Appimage "packages" will need to install this file manually.


Udev rules are built from the source at compile time. 
When building locally they are installed with the make install step to /usr/lib/udev/rules.d/60-openrgb.rules

If you need to install the UDEV rules file manually you can also download the latest compiled udev rules from Gitlab at https://gitlab.com/CalcProgrammer1/OpenRGB.
or clone this repo

Copy this 60-openrgb.rules file to /usr/lib/udev/rules.d/
Then reload rules with : 'sudo udevadm control --reload-rules && sudo udevadm trigger'







