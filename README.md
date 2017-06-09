### credits
Initial mac-layout: bmaeser

# German International Keyboard Layout

A german optimized keyboard-layout (mac / win) (based on US-QWERTY) for programmers and people who use predefined shortcuts on a daily basis.

### the problem(s)

Most programs shortcut mappings are made for the U.S.-layout. That is why some shortcuts won't work on the german layout. This includes technically every key combination that requires an extra key modifier compared to the combination on the U.S.-layout. This is annoying and can only be resolved by defining custom shortcut mappings or using another layout. Unfortunately, the other layouts are missing the German umlauts (ä, ö, ü) as well as other language/region specific symbols (ß, €, °).

Another problem with the German layout is that programmers have a hard time typing important symbols such as parentheses (`[`, `]`, `{`, `}`) and slashes (`/`, `\`) because they are mapped to `alt` + `base key` combinations (`alt` + `7` = `/`). (On Windows `alt` = `Alt Gr`)

### the solution

The solution is the following keyboard-layout based on the U.S. layout containing the missing special characters (like umlauts and so on).

For ANSI and ISO keyboards. 

Essentially its a [us-keyboard-layout](http://en.wikipedia.org/wiki/File:KB_United_States-NoAltGr.svg) (QWERTY) with some alterations:

* your umlauts, `€` and `ß` work with `option-key` / `alt` (win: `AltGr` / `Ctrl` + `Alt`) + base-key:
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

*If you have a better idea for the extra key, let me know*


## Installation (MAC)

#### per user (not available at login screen, no admin rights required)
Unzip `GermanIntl.bundle.zip`, copy `GermanIntl.bundle` into `~/Library/Keyboard Layouts` and pick `German Intl.` (German -> German Intl.) as layout in the language preference pane. A restart may be required.

#### for everyone (admin rights required)
Unzip `GermanIntl.bundle.zip`, copy `GermanIntl.bundle` into `/Library/Keyboard Layouts` and pick `German Intl.` (German -> German Intl.) as layout in the language preference pane. A restart may be required.

## Installation (WIN)

#### for everyone (admin rights required)
Unzip `setup-win.zip`, execute `setup.exe`, goto language settings, click on your language and add keyboard layout `German International`. Make sure the layout is at the top of the list by removing layouts above it.  A restart may be required.

#### per session (portable, no admin rights required, suited for use at public places)
Unzip `portable-win.zip`, execute `pkl.exe`. (Control via tray-icon)

*known bug of the portable win version is that if the currently selected keyboard layout has some deadkeys, these keys will be handled as deadkeys regardless if the key is a deadkey in this layout -> fix: select another layout that has no deadkeys (e.g. US)*

## Layout images (ISO)

### default
![default](https://raw.githubusercontent.com/progmem64/German-International-Keyboard-Layout/master/layout-img/default.png)

### shift
![shift](https://raw.githubusercontent.com/progmem64/German-International-Keyboard-Layout/master/layout-img/shift.png)

### alt (win: AltGr / Ctrl + Alt)
![alt](https://raw.githubusercontent.com/progmem64/German-International-Keyboard-Layout/master/layout-img/alt.png)

### alt + shift (win: AltGr + Shift / Ctrl + Alt + Shift)
![alt + shift](https://raw.githubusercontent.com/progmem64/German-International-Keyboard-Layout/master/layout-img/altshift.png)
