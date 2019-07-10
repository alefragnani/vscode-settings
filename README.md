# VSCode Settings

My personal Visual Studio Code settings.

_I'm keeping it here because I want to have it synced between different machines._

## Preferences / User Settings

* Encoding
* Word Wrap
* Files Exclude
  - Pascal
  - Java
  - FinalBuilder
* Search Exclude
  - Pascal  

## Preferences / Keyboards Shortcuts

Mostly to use the same shortcut for every code editor

## Preferences / User Snippets

* Pascal
* Java
* JSON
* JavaScript
* CoffeScript
* Markdown

## Syncing (using Symlink)

The **symlinks** must be _hard links_, otherwise VS Code will display errors about _to many link loop_ or something like that.

### Windows

#### Stable
```
cd %HOMEPATH%/Documents/GitHub/vscode-settings/
mklink /H %HOMEPATH%\AppData\Roaming\Code\User\settings.json settings.json
mklink /H %HOMEPATH%\AppData\Roaming\Code\User\keybindings.json keybindings.json
mklink /J %HOMEPATH%\AppData\Roaming\Code\User\snippets snippets
```

#### Insiders
```
cd %HOMEPATH%/Documents/GitHub/vscode-settings/
mklink /H "%HOMEPATH%\AppData\Roaming\Code - Insiders\User\settings.json" settings.json
mklink /H "%HOMEPATH%\AppData\Roaming\Code - Insiders\User\keybindings.json" keybindings.json
mklink /J "%HOMEPATH%\AppData\Roaming\Code - Insiders\User\snippets" snippets
```

### MacOS

#### Stable
```
cd ~/Documents/GitHub/vscode-settings/
ln -h settings.json ~/Library/Application\ Support/Code/User/settings.json
ln -h keybindings.json ~/Library/Application\ Support/Code/User/keybindings.json
ln -s ~/Documents/GitHub/vscode-settings/snippets ~/Library/Application\ Support/Code/User/snippets
```

#### Insiders
```
cd ~/Documents/GitHub/vscode-settings/
ln -h settings.json ~/Library/Application\ Support/Code\ -\ Insiders/User/settings.json
ln -h keybindings.json ~/Library/Application\ Support/Code\ -\ Insiders/User/keybindings.json
ln -s ~/Documents/GitHub/vscode-settings/snippets ~/Library/Application\ Support/Code\ -\ Insiders/User/snippets
```