# Extensions

* [Apache Conf](https://marketplace.visualstudio.com/items?itemName=mrmlnc.vscode-apache)
* [Favorites](https://marketplace.visualstudio.com/items?itemName=kdcro101.favorites)
* [Live Sass Compiler](https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass)
* [PHP IntelliSense](https://marketplace.visualstudio.com/items?itemName=felixfbecker.php-intellisense)
* [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
* [Selected Lines Count](https://marketplace.visualstudio.com/items?itemName=gurumukhi.selected-lines-count)
* [Sync Scroll](https://marketplace.visualstudio.com/items?itemName=dqisme.sync-scroll)

# File > Preferences > Settings > Open Settings (JSON)

    "editor.fontSize": 13,
    "editor.tabSize": 4,
    "editor.insertSpaces": true,
    "editor.trimAutoWhitespace": false,
    "workbench.tree.indent": 16,
    "workbench.startupEditor": "newUntitledFile",
    "workbench.colorTheme": "Visual Studio Light",
    "editor.renderControlCharacters": false,
    "php.suggest.basic": false,
    "editor.minimap.enabled": true,
    "workbench.colorCustomizations": {
        "minimap.background" : "#fdfdfd"
    }

# File > Preferences > Keyboard Shortcuts
    
    Copy Line Down          -> Ctrl + D
    Toggle Line Comment     -> Ctrl + Q
    Toggle Block Comment    -> Ctrl + Alt + W

# File > Preferences > [User Snippets](https://code.visualstudio.com/docs/editor/userdefinedsnippets) > PHP

* Show snippets: Ctrl + Space

```
"Section Comment 40" : {
    "prefix" : "sec40",
    "body" : [
        "/* ======================================== $0 ======================================== */"
    ],
    "description": "Add a section comment."
},

"Section Comment 25" : {
    "prefix" : "sec25",
    "body" : [
        "/* ========================= $0 ========================= */"
    ],
    "description": "Add a sub section comment."
}
```