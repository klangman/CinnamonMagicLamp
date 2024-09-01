# CinnamonMagicLamp

A compiz like magic lamp effect for the Cinnamon desktop based on hermes83's Gnome extension (https://github.com/hermes83/compiz-alike-magic-lamp-effect)

![screen shot](CinnamonMagicLamp@klangman/screenshot.png)

This Cinnamon extension will create a compiz like Magic Lamp minimize and unminimize effect

## IMPORTANT

You must disable the Cinnamon Minimize and Unminimize effects as they will interfere with the operation of the Magic Lamp effect. Open the Menu->Preferences->Effects application and set the "New windows or unminimizing existing ones" and "Minimize windows" features to "None".

## Requirements

Cinnamon 5.6.8 (Mint 21.1) or better.

To properly animate in relation to the window-list icon, you need to be using a window-list applet that sets the icon geometry. Otherwise the animation will animate from/to the middle of the monitor on the Cinnamon panel edge rather than an animation specific to the window. The pre-installed "Window list" and "Grouped window list" applets work fine as does "Cassia Window list" (version 2.3.2 or better). CobiWindowList does not currently set icon geometry.

This extension requires no other packages other than what is included in a default installation of Mint 21.1 or better.

## Known issues

The Steam client for some reason does not support window cloning when minimized, therefore the "minimize" effect will show a blank/black window rather than the correct window contents. Other application might have the same behaviour but I have not seen any yet.

## Installation

For the "Stable" version, use the "Extensions" tool from the cinnamon setting, click the "Download" tab and find "Cinnamon Magic Lamp"

For the development version you will need to following these instructions to install manually:

1. Clone the repo (or Download the latest repo by clinking on the green "code" button above then click "Download ZIP")
    ```
    git clone git@github.com:klangman/CinnamonMagicLamp.git
    ```
2. If you downloaded a ZIP, decompress the zip into a directory of your choice
    ```
    unzip ~/Downloads/CinnamonMagicLamp-main.zip
    ```
3. Change directory to the cloned repo or the decompressed ZIP file
4. Link the "CinnamonMagicLamp@klangman" directory into the "~/.local/share/cinnamon/extensions/" directory
    ```
    ln -s $PWD/CinnamonMagicLamp@klangman ~/.local/share/cinnamon/extensions/CinnamonMagicLamp@klangman
    ```
5. Open the Cinnamon Extensions application (Menu->Preferences->Extensions)
6. Select the "Magic Lap Effect" entry and then click the "+" button at the bottom of the Extensions window
7. **Important:** Open the Menu->Preferences->Effects application and change the Minimize and Unminimize effect options to "None"
8. Use the "gears" icon to open the CinnamonMagicLamp setting window and setup the preferred behaviour

## Feedback

Feel free to create an issue here on Github to give me feedback or to report any issues you find.

If you like this extension, please star it so that more people might learn of it's existence.
Also, the more stars it gets the more encouragement I'll have to continue working on it.
Thanks!

Icon based on an icon by Nikita Golubev (https://www.flaticon.com/free-icon/magic-lamp_1065505)
