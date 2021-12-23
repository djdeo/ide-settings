# IDE-settings
VScode and Sublime settings
## VScode settings

```json
{
  "explorer.confirmDelete": false,
  "editor.suggestSelection": "first",
  "material-icon-theme.folders.color": "#42a5f5",
  "material-icon-theme.folders.theme": "specific",
  "workbench.iconTheme": "material-icon-theme",
  "editor.fontFamily": "JetBrains Mono, Operator Mono, Consolas, 'Courier New', monospace",
  "editor.fontLigatures": true,
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "typescript",
    "typescriptreact"
  ],
  "editor.tabSize": 2,
  "typescript.format.enable": false,
  "javascript.validate.enable": false,
  "[javascript, vue]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "editor.quickSuggestions": {
    "strings": true
  },
  "git.confirmSync": false,
  "git.autofetch": true,
  "git.enableSmartCommit": true,
  "editor.fontSize": 13,
  "workbench.colorTheme": "Night Wolf [gray] (No Italics)",
  "terminal.explorerKind": "external",
  "terminal.external.osxExec": "iTerm.app",
  "terminal.integrated.localEchoStyle": "dim",
  "terminal.integrated.fontSize": 13,
  "liveServer.settings.donotShowInfoMsg": true,
  "files.trimTrailingWhitespace": true,
  "bracket-pair-colorizer-2.depreciation-notice": false,
  "javascript.format.insertSpaceAfterFunctionKeywordForAnonymousFunctions": false,
  "typescript.format.insertSpaceAfterFunctionKeywordForAnonymousFunctions": false,
  "editor.formatOnSaveMode": "modifications",
  "html.format.preserveNewLines": false,
  "eslint.codeActionsOnSave": true, // 每次保存的时候将代码按eslint格式进行修复
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  "editor.formatOnSave": true,
  "editor.formatOnType": true,
  "prettier.eslintIntegration": true, //让prettier使用eslint的代码格式进行校验
  "prettier.semi": false, //去掉代码结尾的分号
  "prettier.singleQuote": true, //使用单引号替代双引号
  // "javascript.format.insertSpaceBeforeFunctionParenthesis": true, //让函数(名)和后面的括号之间加个空格
  "vetur.format.defaultFormatter.html": "js-beautify-html", //格式化.vue中html
  "vetur.format.defaultFormatter.js": "vscode-typescript", //让vue中的js按编辑器自带的ts格式进行格式化
  "vetur.format.defaultFormatterOptions": {
    "js-beautify-html": {
      "wrap_attributes": "force-aligned" //属性强制折行对齐
    }
  },
  "tabnine.experimentalAutoImports": true,
  "editor.inlineHints.fontFamily": "Operator Mono, Menlo, Monaco, 'Courier New', monospace",
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "errorLens.fontFamily": "Operator Mono",
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

## Sublime JavaScript Build (F7)

Tools > Build System > New Build System…   and save as `JavaScript.sublime-build`

### Mac

```json
{
  "cmd": ["/usr/local/bin/node", "$file"],
  "selector": "source.js"
}
```

### Windows 

```json
{
  "cmd": ["C:/Program Files/nodejs/node.exe", "$file"],
  "selector": "source.js"
}
```
