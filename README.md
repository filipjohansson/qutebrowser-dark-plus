# Dark+ Theme for [Qutebrowser](https://www.qutebrowser.org/)

A [Qutebrowser](https://www.qutebrowser.org/) theme inspired by the [Dark+ VS Code theme](https://github.com/microsoft/vscode/blob/main/extensions/theme-defaults/themes/dark_plus.json).

_General structure and inspiration taken from [Qutebrowser Dracula theme](https://github.com/dracula/qutebrowser/)._

## Installation

### 1. Locate your Qutebrowser configuration directory
The typical [Qutebrowser configuration directories](https://www.qutebrowser.org/doc/help/configuring.html#configpy) are `~/.config/qutebrowser/` on Linux, `~/.qutebrowser/` on macOS, and `%APPDATA%/qutebrowser/config/` on Windows. If you are unable to locate your configuration directory you can run `:version` in Qutebrowser, the value under Path: > config: is your configuration directory.

### 2. Get the theme
#### a. Install using Git
Clone the repository into your configuration directory, in the example below we assume you are using the default directory on Linux, you should change it to match your OS.

_If your configuration folder is already in Git you could use [Git Submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules) instead._

`git clone https://github.com/filipjohansson/qutebrowser-dark-plus.git ~/.qutebrowser/dark_plus`

#### b. Manual install
Download the zip from Github and unzip it into your configuration directory.

### 3. Activate the theme

```python
import dark_plus.draw

dark_plus.draw.dark(c, {
    'spacing': {
        'vertical': 5,
        'horizontal': 5
    }
})
```
