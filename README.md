Et un grand merci à Tiheum pour toutes ses icones/thèmes !

Installation
============

Install git with : 

    sudo apt-get install git


=======
Extra configuration
===================
## Firefox
If you are a Firefox user, you may also appreaciate [~illusionmist Holo Stylish script for Firefox](http://illusionmist.deviantart.com/art/Holo-Theme-for-Firefox-294051732)

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
It's because they try to use _Roboto_ instead of Light variant and it will appear bold for you.    
So, you have to force the resolution of _Roboto_ into _Roboto Light_ instead of _Roboto Medium_.
So edit your ```~/.fonts.conf``` and fill with :

```xml
<?xml version="1.0"?>
<!DOCTYPE fontconfig SYSTEM "fonts.dtd">
<fontconfig>
    <match target="pattern">
        <test name="family" qual="any">
            <string>Roboto</string>
        </test>
        <edit mode="assign" name="family">
            <string>Roboto Light</string>
        </edit>
    </match>
</fontconfig>
```

Finally, you can then use gnome-tweak-tool to setup everything.


----

Remember that the Holo theme is released under GPLv3 license.
And don't hesitate to share if you modify for your own needs ;).
