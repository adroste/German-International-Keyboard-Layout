### Credits
Initial mac-layout: bmaeser


# coDE
A german optimized keyboard-layout (mac / win) for programmers (based on US-QWERTY).

Works on ANSI and ISO keyboards.

Essentially its a [us-keyboard-layout](http://en.wikipedia.org/wiki/File:KB_United_States-NoAltGr.svg) with some alterations:

* `Z` and `Y` are are swapped. (QWERTZ)
* your umlauts, `€` and `ß` work with `option-key` / `alt` (win: `AltGr`) + base-key:
    * `alt` + `A` = `ä`
    * `alt` + `shift` + `A` = `Ä`
    * `alt` + `O` = `ö`
    * `alt` + `shift` + `O` = `Ö`
    * `alt` + `U` = `ü`
    * `alt` + `shift` + `U` = `Ü`
    * `alt` + `S` = `ß`
    * `alt` + `E` = `€`
* `~` (tilde / unix-home) is on two places:
    * `shift` + `` ` `` (us-standard)
    * on the extra key on ISO-keyboards, between `left-shift` and `Y` (extra key: yay!)
* `°` (degree) is on `shift` + the extra ISO-key (between `left-shift` and `Y`)
* all dead-keys are disabled, so if you hit `` ` ``, `~` or `^` you get `` ` ``, `~` or `^`
* 'period' on the numblock produces `,` not `.`


### Installation (MAC)

#### per user (not available at login screen, no admin rights required)
Unzip `coDE.bundle.zip`, copy `coDE.bundle` into `~/Library/Keyboard Layouts` and pick `coDE` (German -> coDE) as layout in the preference pane. A restart may be required.

#### for everyone (admin rights required)
Unzip `coDE.bundle.zip`, copy `coDE.bundle` into `/Library/Keyboard Layouts` and pick `coDE` (German -> coDE) as layout in the preference pane. A restart may be required.


### Installation (WIN)

#### for everyone (admin rights required)
Unzip `setup-win.zip`, execute `setup.exe` and pick layout `Deutsch (Lichtenstein) - coDE German Programming Layout`. A restart may be required.

#### per session (portable, no admin rights required, suited for use at public places)
Unzip `portable-win.zip`, execute `pkl.exe`. (Control via tray-icon)


### Layout Images (ISO)

### default
![default](https://raw.githubusercontent.com/progmem64/coDE/master/layout-img/default.png)

### shift
![shift](https://raw.githubusercontent.com/progmem64/coDE/master/layout-img/shift.png)

### alt (win: AltGr, only umlauts for now)
![alt](https://raw.githubusercontent.com/progmem64/coDE/master/layout-img/alt.png)

### alt + shift (win: AltGr + Shift, only umlauts for now)
![alt + shift](https://raw.githubusercontent.com/progmem64/coDE/master/layout-img/altshift.png)
