# Material Shell
## A material tiling shell replacement for GNOME Shell to simplify your workflow and accelerate your productivity.

The project is based on my earlier work on [Material Awesome](https://github.com/PapyElGringo/material-awesome). This GNOME Shell extension provides a performant, opinionated mouse/keyboard workflow and follows the [Material Design guidelines](https://material.io).

## Demo

![Demo GIF](demo.gif)

### Discord
Get notified about updates and join me at [https://discord.gg/vBb7D9a](https://discord.gg/vBb7D9a)
#
#### STATUS: BETA (expect bugs!)
#### REQUIRES: gnome-shell >=3.32.0

## Installation
1) Clone the project to the gnome-shell extensions folder:
```bash
git clone https://github.com/PapyElGringo/material-shell.git ~/.local/share/gnome-shell/extensions/material-shell@papyelgringo
```
2) Reload GNOME Shell by hitting `Alt+F2` and typing the command `r`
3) Open `gnome-tweaks` and activate `Material-shell` extension **OR** enable it using 
```bash
gnome-shell-extension-tool -e material-shell@papyelgringo
```

## Modifying the Stylesheet
The stylesheet is written in [Sass](https://sass-lang.com) so it must be compiled before it can be reloaded.
First, make sure to install the Sass command line tool with `npm`:
```bash
npm install -g sass
```
If Sass is installed, then:
1) Make changes to the `stylesheet.scss` file as you please.
2) Compile the file, and generate a sourcemap:
```bash
cd ~/.local/share/gnome-shell/extensions/material-shell@papyelgringo
sass stylesheet.scss:stylesheet.css --sourcemap
```
3) Reload GNOME Shell by hitting `Alt+F2` and typing the command `r`

## Workflow Hotkeys
Some hotkeys might already be used by GNOME Shell - please check your keybindings first.
#### Desktop navigation
* `Super+W` Navigate to the upper workspace/category.
* `Super+S` Navigate to the lower workspace/category.
* `Super+A` Focus the window at the left of the current window.
* `Super+D` Focus the window at the right of the current window.

#### Window manipulation
* `Super+Q` Kill the current window focused.
* `Super+[MouseDrag]` Move window around.

#
## Optional Configuration
* Get [Plata Theme](https://gitlab.com/tista500/plata-theme) as the GTK and shell theme 
* Get [Tela Icon Theme](https://github.com/vinceliuice/Tela-icon-theme) as the icon theme
