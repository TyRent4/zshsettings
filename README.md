# Manual TODOS:
#### Manual font installation

1. Download these four ttf files:
   - [MesloLGS NF Regular.ttf](
       https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf)
   - [MesloLGS NF Bold.ttf](
       https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold.ttf)
   - [MesloLGS NF Italic.ttf](
       https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Italic.ttf)
   - [MesloLGS NF Bold Italic.ttf](
       https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold%20Italic.ttf)
1. Double-click on each file and click "Install". This will make `MesloLGS NF` font available to all
   applications on your system.
1. Configure your terminal to use this font:
   - **iTerm2**: Type `p10k configure` and answer `Yes` when asked whether to install
     *Meslo Nerd Font*. Alternatively, open *iTerm2 → Preferences → Profiles → Text* and set *Font* to
     `MesloLGS NF`.
   - **Apple Terminal**: Open *Terminal → Preferences → Profiles → Text*, click *Change* under *Font*
     and select `MesloLGS NF` family.
   - **Hyper**: Open *Hyper → Edit → Preferences* and change the value of `fontFamily` under
     `module.exports.config` to `MesloLGS NF`.
   - **Visual Studio Code**: Open *File → Preferences → Settings* (PC) or
     *Code → Preferences → Settings* (Mac), enter `terminal.integrated.fontFamily` in the search box at
     the top of *Settings* tab and set the value below to `MesloLGS NF`.
     Consult [this screenshot](
       https://raw.githubusercontent.com/romkatv/powerlevel10k-media/389133fb8c9a2347929a23702ce3039aacc46c3d/visual-studio-code-font-settings.jpg)
     to see how it should look like or see [this issue](
       https://github.com/romkatv/powerlevel10k/issues/671) for extra information.
   - **GNOME Terminal** (the default Ubuntu terminal): Open *Terminal → Preferences* and click on the
     selected profile under *Profiles*. Check *Custom font* under *Text Appearance* and select
     `MesloLGS NF Regular`.
   - **Konsole**: Open *Settings → Edit Current Profile → Appearance*, click *Select Font* and select
     `MesloLGS NF Regular`.
   - **Tilix**: Open *Tilix → Preferences* and click on the selected profile under *Profiles*. Check
     *Custom font* under *Text Appearance* and select `MesloLGS NF Regular`.
   - **Windows Console Host** (the old thing): Click the icon in the top left corner, then
     *Properties → Font* and set *Font* to `MesloLGS NF`.
   - **Windows Terminal** by Microsoft (the new thing): Open *Settings* (<kbd>Ctrl+,</kbd>), click
     either on the selected profile under *Profiles* or on *Defaults*, click *Appearance* and set
     *Font face* to `MesloLGS NF`.
   - **IntelliJ** (and other IDEs by Jet Brains): Open *IDE → Edit → Preferences → Editor →
     Color Scheme → Console Font*. Select *Use console font instead of the default* and set the font
     name to `MesloLGS NF`.
   - **Termux**: Type `p10k configure` and answer `Yes` when asked whether to install
     *Meslo Nerd Font*.
   - **Blink**: Type `config`, go to *Appearance*, tap *Add a new font*, tap *Open Gallery*, select
     *MesloLGS NF.css*, tap *import* and type `exit` in the home view to reload the font.
   - **Terminus**: Open *Settings → Appearance* and set *Font* to `MesloLGS NF`.
   - **Terminator**: Open *Preferences* using the context menu. Under *Profiles* select the *General*
     tab (should be selected already), uncheck *Use the system fixed width font* (if not already)
     and select `MesloLGS NF Regular`. Exit the Preferences dialog by clicking *Close*.
   - **Guake**: Right Click on an open terminal and open *Preferences*. Under *Appearance*
     tab, uncheck *Use the system fixed width font* (if not already) and select `MesloLGS NF Regular`.
     Exit the Preferences dialog by clicking *Close*.
   - **MobaXterm**: Open *Settings* → *Configuration* → *Terminal* → (under *Terminal look and feel*)
     and change *Font* to `MesloLGS NF`.
   - **Asbrú Connection Manager**: Open *Preferences → Local Shell Options → Look and Feel*, enable
     *Use these personal options* and change *Font:* under *Terminal UI* to `MesloLGS NF Regular`.
     To change the font for the remote host connections, go to *Preferences → Terminal Options →
     Look and Feel* and change *Font:* under *Terminal UI* to `MesloLGS NF Regular`.
   - **WSLtty**: Right click on an open terminal and then on *Options*. In the *Text* section, under
     *Font*, click *"Select..."* and set Font to `MesloLGS NF Regular`.
   - **Yakuake**: Click *≡* → *Manage Profiles* → *New* → *Appearance*. Click *Choose* next to the
     *Font* dropdown, select `MesloLGS NF` and click *OK*. Click *OK* to save the profile. Select the
     new profile and click *Set as Default*.
   - **Alacritty**: Create or open `~/.config/alacritty/alacritty.yml` and add the following section
     to it:
     ```yaml
     font:
       normal:
         family: "MesloLGS NF"
     ```
    - **kitty**: Create or open `~/.config/kitty/kitty.conf` and add the following line to it:
      ```text
      font_family MesloLGS NF
      ```
      Restart kitty by closing all sessions and opening a new session.
   - **puTTY**: Set *Window* → *Appearance* → *Font* to `MesloLGS NF`. Requires puTTY
     version >= 0.75.
   - **WezTerm**: Create or open `$HOME/.config/wezterm/wezterm.lua` and add the following:
     ```lua
     local wezterm = require 'wezterm';
     return {
         font = wezterm.font("MesloLGS NF"),
     }
     ```
     If the file already exists, only add the line with the font to the existing return.
     Also add the first line if it is not already present.
   - **urxvt**: Create or open `~/.Xresources` and add the following line to it:
     ```text
     URxvt.font: xft:MesloLGS NF:size=11
     ```
     You can adjust the font size to your preference. After changing the config run
     `xrdb ~/.Xresources` to reload it. The new config is applied to all new terminals.
   - **xterm**: Create or open `~/.Xresources` and add the following line to it:
     ```text
     xterm*faceName: MesloLGS NF
     ```
     After changing the config run `xrdb ~/.Xresources` to reload it. The new config is applied to
     all new terminals.
   - Crostini (Linux on Chrome OS): Open
     chrome-untrusted://terminal/html/nassh_preferences_editor.html, set *Text font family* to
      `'MesloLGS NF'` (including the quotes) and *Custom CSS (inline text)* to the following:
     ```css
     @font-face {
      font-family: "MesloLGS NF";
      src: url("https://raw.githubusercontent.com/romkatv/powerlevel10k-media/master/MesloLGS%20NF%20Regular.ttf");
      font-weight: normal;
      font-style: normal;
     }
     @font-face {
         font-family: "MesloLGS NF";
         src: url("https://raw.githubusercontent.com/romkatv/powerlevel10k-media/master/MesloLGS%20NF%20Bold.ttf");
         font-weight: bold;
         font-style: normal;
     }
     @font-face {
         font-family: "MesloLGS NF";
         src: url("https://raw.githubusercontent.com/romkatv/powerlevel10k-media/master/MesloLGS%20NF%20Italic.ttf");
         font-weight: normal;
         font-style: italic;
     }
     @font-face {
         font-family: "MesloLGS NF";
         src: url("https://raw.githubusercontent.com/romkatv/powerlevel10k-media/master/MesloLGS%20NF%20Bold%20Italic.ttf");
         font-weight: bold;
         font-style: italic;
     }
     ```
     **_CAVEAT_**: If you open the normal terminal preferences these settings will be overwritten.
1. Run `p10k configure` to generate a new `~/.p10k.zsh`. The old config may work
   incorrectly with the new font.
