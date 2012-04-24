Holo-Gnome3-Theme
=================

Holo theme for gnome shell.

Based on the excellent work from Tiheum.
[Holo theme on DeviantArt](http://tiheum.deviantart.com/art/Holo-280076980)

This repository helps to have Gnome 3.4 working with this Holo theme.

It doesn't aim to be backward compatible with Gnome 3.2.

Remember that the Holo theme is released under GPLv3 license.
And don't hesitate to share if you modify for your own needs ;).

Et un grand merci à Tiheum pour toutes ses icones/thèmes !

Installation
============
To install it directly using command line :

    # Install git (if not already)
    sudo apt-get install git
    # Create .themes folder (if not already)
    mkdir ~/.themes
    # Checkout git repo
    cd ~/.themes && git clone git://github.com/r3gis3r/Holo-Gnome3-Theme.git
    # Optionally link root theme folder to your folder
    sudo ln -s ~/.themes ~root/.themes

Extra links
===========
 * If you are a Firefox user, you may also appreaciate [~illusionmist Holo Stylish script for Firefox](http://illusionmist.deviantart.com/art/Holo-Theme-for-Firefox-294051732)
 * You may also want to install Roboto fonts

To do so use following command lines :

    # Get roboto fonts
    wget http://www.fontsquirrel.com/fonts/download/roboto -O roboto.zip
    # Create .fonts theme (if not already)
    mkdir ~/.fonts
    # Unzip fonts in folder
    unzip roboto.zip -d ~/.fonts

You can then use gnome-tweak-tool to setup everything.