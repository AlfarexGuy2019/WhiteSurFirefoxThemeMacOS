## Firefox WhiteSur theme

<p align="center">A <code>MacOS</code> & <code>Windows</code> Firefox theme to look more like Big Sur Safari. (For Firefox 70+)</p>

#### Preview
![Preview](whitesur.gif?raw=true)

## Description

Aim is to make Firefox look more like MacOS Big Sur Safari.
This is a CSS theme adapted to work on MacOS from the Linux GTK theme.
Based on https://github.com/vinceliuice/WhiteSur-gtk-theme/tree/master/src/other/firefox
(This is a quick modification, and is not written from scratch.)

## Installation (MacOS)

Download the latest [release](https://github.com/AdamXweb/WhiteSurFirefoxThemeMacOS/releases/), or clone the repo above.
A script has been added to streamline the installation process.\
Open terminal in the directory of the repo, and run `bash install.sh`\
Follow the prompts

### Manual installation (MacOS & Windows)

Copy `chrome` and `configuration` folers into your Firefox Profile Directory

To find your Firefox Profile Directory you can:

1. Go to `about:support` in Firefox.
2. Application Basics > Profile Directory > Open Directory.
3. Copy folders mentioned above into the profile folder. (usually has `-release` at the end).
4. If you are using Firefox 69+:
	1. Go to `about:config` in Firefox.
	2. Search for `toolkit.legacyUserProfileCustomizations.stylesheets` and set it to `true`.
5. Restart Firefox.
6. Done!

### Manual colour override:

The theme obeys your system UI colour preferences. If you want to override it e.g. always have the dark theme, then you'll have to do the following.\
The solution if you don't want to change your System UI colour is to do add the following to your `about:config`\
Add: `ui.systemUsesDarkTheme` with the number value with 1 for dark, and 0 for light.\
![Screen Shot 2021-05-04 at 7 10 19 pm](https://user-images.githubusercontent.com/6800453/116982626-60317980-ad0c-11eb-96aa-0879b05c98fc.png)


## Known bugs

If it is a fresh install of Firefox, the script's user profile should enable the theme automatically. As a backup, the `pref.js` toggles the setting to enable custom themes.
If for any reason the WhiteSur theme doesn't activate after using the script, follow steps 4.1 and 4.2 to toggle the stylesheets from within the Firefox settings.

The tab background colour is overwritten by themes installed.
e.g. if you are using a dark theme in light mode, tab backgrounds that are inactive are affected.
Fix: Change the installed theme to appropriate colour scheme to avoid issues.

If you're looking to change the directory to run the script, you can always type `bash` then drag the file into terminal, otherwise type `cd` and then drag the folder in and press enter.\
Alternatively, if you're running Catalina, the default teminal is zsh, meaning you can change folders by typing the name to enter the folder e.g. `WhiteSurFirefoxThemeMacOS`


Q: "Why bother doing this, and not just use safari?"
A: I've used safari for quite a few years, and was rather disappointed with the change in extensions, particularly with content blocking. This prompted me to use uBlock origin on Firefox, and to customise it to have the best aesthetics, and simplest transition.

### New bugs

If you've found a new bug, please report it as a new issue with the following:

1. OS you're using
2. Version of Firefox
3. Screenshot of bug if possible
4. Description

Thanks!

## Screenshot

### Windows
![Preview](whitesurwindows.gif?raw=true)


### MacOS
![Preview](whitesur.gif?raw=true)

