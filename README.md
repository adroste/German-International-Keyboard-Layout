### credits
Initial mac-layout: bmaeser

# German International Keyboard Layout

A german optimized keyboard-layout (mac / win / linux) (based on US-QWERTY) for programmers and people who use predefined shortcuts on a daily basis.

### the problem(s)

Most programs shortcut mappings are made for the U.S.-layout. That is why some shortcuts won't work on the german layout. This includes technically every key combination that requires an extra key modifier compared to the combination on the U.S.-layout. This is annoying and can only be resolved by defining custom shortcut mappings or using another layout. Unfortunately, the other layouts are missing the German umlauts (ä, ö, ü) as well as other language/region specific symbols (ß, €, °).

Another problem with the German layout is that programmers have a hard time typing important symbols such as parentheses (`[`, `]`, `{`, `}`) and slashes (`/`, `\`) because they are mapped to `alt` + `base key` combinations (`alt` + `7` = `/`). (On Windows `alt` = `Alt Gr`)

### the solution

The solution is the following keyboard-layout based on the U.S. layout containing the missing special characters (like umlauts and so on).

For ANSI and ISO keyboards. 

### the layout

Essentially its a [us-keyboard-layout](http://en.wikipedia.org/wiki/File:KB_United_States-NoAltGr.svg) (QWERTY) with some alterations:

*In the following context the term `alt` is used for the following modifier combinations:*
*mac: `option-key` / `alt`*
*win: `AltGr` / `Ctrl` + `Alt`*
*linux: `AltGr` / `Right Alt` (other combinations like left alt key can also be used as explained further below)*

* your umlauts, `€` and `ß` work with:
    * `alt` + `A` = `ä`
    * `alt` + `shift` + `A` = `Ä`
    * `alt` + `O` = `ö`
    * `alt` + `shift` + `O` = `Ö`
    * `alt` + `U` = `ü`
    * `alt` + `shift` + `U` = `Ü`
    * `alt` + `S` = `ß`
    * `alt` + `E` = `€`
* some of the dead-keys are disabled, so if you hit `` ` ``, `~` or `^` you get `` ` ``, `~` or `^`
* special on ISO-keyboards (the ones with the extra key between `left shift` and `z` (QWERTY) or `y` (QWERTZ)):
    * the extra key produces `§`
    * `°` (degree symbol) is on `shift` + `§`

*If you have a better idea for the extra key (or other key combinations), let me know*


## Installation (MAC)

#### per user (not available at login screen, no admin rights required)
1. unzip `GermanIntl.bundle.zip`
2. copy `GermanIntl.bundle` into `~/Library/Keyboard Layouts`
3. *(a restart may be required)*
4. pick `German Intl.` (German -> German Intl.) as layout in the language preference pane.

#### for everyone (admin rights required)
1. unzip `GermanIntl.bundle.zip`
2. copy `GermanIntl.bundle` into `/Library/Keyboard Layouts` 
3. *(a restart may be required)*
4. pick `German Intl.` (German -> German Intl.) as layout in the language preference pane. 

## Installation (WIN)

#### for everyone (admin rights required)
1. unzip `setup-win.zip`
2. execute `setup.exe`
3. *(a restart may be required)*
4. select the keyboard layout:
   goto language settings, click on your language, hit options/edit (just click on your current language, do not add a new display language) and add keyboard layout `German International`. Make sure the layout is at the top of the list by removing layouts above it.  

#### per session (portable, no admin rights required, suited for use at public places)
1. unzip `portable-win.zip`
2. execute `pkl.exe`. (Control via tray-icon)

*known bug of the portable win version is that if the currently selected keyboard layout has some deadkeys, these keys will be handled as deadkeys regardless if the key is a deadkey in this layout -> fix: select another layout that has no deadkeys (e.g. US)*

## Installation (LINUX)

The layout was made for Ubuntu 16.04. It should also work on similiar systems using X11-KBD … like Ubuntu 14.04, 16.10, 17.04, … :), just try it out and report if something is broken

#### for everyone (root / sudo rights required)

1. add the layout:
   Unzip `GermanIntl-ubuntu.zip` and copy `gerintl` into `/usr/share/X11/xkb/symbols`. 
2. create the layout definition:
   The The next step is more difficult than on other systems, but it should be easy for someone who is using linux on its desktop: Copy the layout-rule found in `evdev-rule.xml` and paste it into `/usr/share/X11/xkb/rules/evdev.xml` between the last `</layout>` closing tag and the `</layoutList>` closing tag. Just do not mess up your layout config file. I did it, just do not do it.
3. reconfigure your xkb-date by executing `sudo dpkg-reconfigure xkb-data`
4. *(a restart may be required)*
5. select the keyboard layout:
   Goto Settings > Text Entry > + > Add "German International"

#### using different modifiers

By default the right alt key is used to enable the third layout level. You can change the used modifiers by replacing the last line of the `gerintl ` file from `"level3(ralt_switch)"` to a different modifier mapping. 

E.g.: to use the left alt key only: `include "level3(lalt_switch)"` or to use both alt keys (like on a mac): `include "level3(alt_switch)"`

For a more specific mapping, please have a look at `/usr/share/X11/xkb/symbols/level3`.

## Layout images (ISO)

### default
![default](https://raw.githubusercontent.com/progmem64/German-International-Keyboard-Layout/master/layout-img/default.png)

### shift
![shift](https://raw.githubusercontent.com/progmem64/German-International-Keyboard-Layout/master/layout-img/shift.png)

### alt
![alt](https://raw.githubusercontent.com/progmem64/German-International-Keyboard-Layout/master/layout-img/alt.png)

### alt + shift
![alt + shift](https://raw.githubusercontent.com/progmem64/German-International-Keyboard-Layout/master/layout-img/altshift.png)

*the Apple symbol is a heart ♥ on windows and linux*