# IDE-settings
VScode and Sublime settings
## VScode settings

```json
{
    "liveServer.settings.donotVerifyTags": true,
    "liveServer.settings.donotShowInfoMsg": true,
    "workbench.colorTheme": "Ayu Mirage",
    "window.zoomLevel": 1,
    "editor.fontSize": 16,
    "editor.lineHeight": 35,
    "editor.mouseWheelScrollSensitivity": 2.5,
    "editor.wordWrap": "on",
}
```


## VScode shortcut blinding:

```json
[
    {
        "key": "ctrl+shift+oem_1",
        "command": "editor.emmet.action.removeTag"
    },
    {
        "key": "ctrl+shift+alt+s",
        "command": "workbench.action.files.saveAll"
    },
    {
        "key": "ctrl+k s",
        "command": "-workbench.action.files.saveAll"
    },
    {
        "key": "ctrl+i",
        "command": "-expandLineSelection",
        "when": "editorTextFocus"
    },
    {
        "key": "alt+f3",
        "command": "editor.action.changeAll",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "ctrl+f2",
        "command": "-editor.action.changeAll",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "shift+alt+w",
        "command": "editor.emmet.action.wrapIndividualLinesWithAbbreviation"
    },
    {
        "key": "ctrl+shift+a",
        "command": "editor.action.smartSelect.grow",
        "when": "editorTextFocus"
    },
    {
        "key": "shift+alt+right",
        "command": "-editor.action.smartSelect.grow",
        "when": "editorTextFocus"
    }
]
```

## Sublime settting

```json
{
    "color_scheme": "Packages/Material Theme/schemes/Material-Theme.tmTheme",
    "font_size": 15,
    "line_padding_bottom": 10,
    "line_padding_top": 10,
    "theme": "Default.sublime-theme"
}
```

## Sublime shortcut

```json
{
    "keys": ["alt+z"],
    "command": "toggle_setting",
    "args": {
        "setting": "word_wrap"
    }
}
```
use `alt+z` to toggle word wrap, like in VScode
