# bookmarks.yazi

A [Yazi](https://github.com/sxyazi/yazi) plugin that allow you to 
save last open path, and jump to last open path at next time.

> [!NOTE]
> The latest main branch of Yazi is required at the moment.


https://github.com/DreamMaoMao/bookmarks.yazi/assets/30348075/cb47efd0-7567-456c-8224-c7ae41130b34


## Installation

```sh
# Linux/macOS
git clone https://gitee.com/DreamMaoMao/lastopen.yazi.git ~/.config/yazi/plugins/bookmarks.yazi

# Windows
git clone https://gitee.com/DreamMaoMao/lastopen.yazi.git $env:APPDATA\yazi\config\plugins\lastopen.yazi
```

## Usage

Add this to your `keymap.toml`:

```toml
[[manager.prepend_keymap]]
on = [ "<Enter>" ]
run = "plugin lastopen --args='open'"
desc = "open file and save path"

[[manager.prepend_keymap]]
on = [ "u", "l" ]
run = "plugin lastopen --args='jump'"
desc = "Jump to lastopen path"

```
