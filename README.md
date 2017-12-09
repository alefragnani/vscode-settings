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