Holo theme for gnome shell & gtk 3.4

 > Based on the excellent work from Tiheum : [Holo theme on DeviantArt](http://tiheum.deviantart.com/art/Holo-280076980)     
 > This repository helps to have Gnome 3.4 working with this Holo theme.     
 > It doesn't aim to be backward compatible with Gnome 3.2.

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


Extra configuration
===================
## Firefox
If you are a Firefox user, you may also appreciate [~illusionmist Holo Stylish script for Firefox](http://illusionmist.deviantart.com/art/Holo-Theme-for-Firefox-294051732)

## Thunderbird
And the thunderbird script [my Holo Stylish script for Thunderbird](http://userstyles.org/styles/64593/holo-theme-for-thunderbird-linux-thunderbir-11?r=1335276031)

## Fonts
You may also want to install Roboto fonts

To do so use following command lines :

    # Get roboto fonts
    wget http://www.fontsquirrel.com/fonts/download/roboto -O roboto.zip
    # Create .fonts theme (if not already)
    mkdir ~/.fonts
    # Unzip fonts in folder
    unzip roboto.zip -d ~/.fonts

If you plan to use _Roboto Light_ instead of _Roboto_, you'll notice weird behavior from apps such as Thunderbird and Pidgin.     
It's because they try to use _Roboto_ in weight normal which resolves to Medium style and it will appear bold for you.    
So, you have to force the resolution of _Roboto_ into _Roboto Light_ for _normal_ weight.
So edit your ```~/.fonts.conf``` and fill with :

```xml
<?xml version="1.0"?>
<!DOCTYPE fontconfig SYSTEM "fonts.dtd">
<fontconfig>
    <match target="pattern">
        <test name="family" qual="any">
            <string>Roboto</string>
        </test>
        <test name="weight" qual="more_eq">
            <string>80</string>
        </test>
        <edit mode="assign" name="style">
            <string>Light</string>
        </edit>
    </match>
</fontconfig>

```

Finally, you can then use gnome-tweak-tool to setup everything.


----

Remember that the Holo theme is released under GPLv3 license.
And don't hesitate to share if you modify for your own needs ;).
