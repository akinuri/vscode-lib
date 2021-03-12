# vscode-lib

Collection of modifications to VS Code.

<br>

## Extensions

Keyboard Shortcut: `Ctrl + Shift + X`

* [Apache Conf](https://marketplace.visualstudio.com/items?itemName=mrmlnc.vscode-apache)
* [Favorites](https://marketplace.visualstudio.com/items?itemName=kdcro101.favorites)
* [Live Sass Compiler](https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass)
* [PHP IntelliSense](https://marketplace.visualstudio.com/items?itemName=felixfbecker.php-intellisense)
* [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
* [Selected Lines Count](https://marketplace.visualstudio.com/items?itemName=gurumukhi.selected-lines-count)
* [Sync Scroll](https://marketplace.visualstudio.com/items?itemName=dqisme.sync-scroll)

<br>

## File > Preferences > Settings > Open Settings (JSON)

Keyboard Shortcut: `Ctrl + ,` `->` `Open Settings (JSON)`

    "editor.fontSize": 13,
    "editor.tabSize": 4,
    "editor.insertSpaces": true,
    "editor.trimAutoWhitespace": false,
    "workbench.tree.indent": 16,
    "workbench.startupEditor": "newUntitledFile",
    "workbench.colorTheme": "Visual Studio Light",
    "editor.renderControlCharacters": false,
    "php.suggest.basic": false,
    "editor.snippetSuggestions" : "top",
    "editor.minimap.enabled": true,
    "editor.autoIndent": "advanced",
    "workbench.colorCustomizations": {
        "minimap.background" : "#fdfdfd"
    },

<br>

## File > Preferences > Keyboard Shortcuts

Keyboard Shortcut: `Ctrl + K Ctrl + S`
    
    Copy Line Down              -> Ctrl + D
    Toggle Line Comment         -> Ctrl + Q
    Toggle Block Comment        -> Ctrl + Alt + W
    Emmet: Go to Matching Pair  -> Ctrl + Alt + D
    Fold All Regions            -> Ctrl + R
    Unfold All Regions          -> Alt + R

<br>

## File > Preferences > [User Snippets](https://code.visualstudio.com/docs/editor/userdefinedsnippets)

Show snippets in editor: `Ctrl + Space`

### PHP

```
"Region Comment (40 dashes)" : {
    "prefix" : "#region40",
    "body" : [
        "#region ======================================== $0 ========================================"
    ],
    "description": "Add a region/section."
},
	
"Method" : {
    "prefix" : "method",
    "body" : [
        "public function methodName(\\$var) {",
        "    $0",
        "}",
    ],
    "description": "Add a class method."
},
```

### HTML

```
"anchor" : {
    "prefix" : "anchor",
    "body" : [
        "<a href=\"#\">$0</a>",
    ],
    "description": "Add an anchor element."
},

"bootstrap button" : {
    "prefix" : "bs.button",
    "body" : [
        "<button type=\"button\" class=\"btn btn-primary\">$0</button>",
    ],
    "description": "Add a col element."
},

"bootstrap button icon" : {
    "prefix" : "bs.button.icon",
    "body" : [
        "<button type=\"button\" class=\"btn btn-primary has-icon\">",
        "    <span class=\"icon\">",
        "        <i class=\"fas fa-save\"></i>",
        "    </span>",
        "    <span>$0</span>",
        "</button>",
    ],
    "description": "Add a col element."
},

"bootstrap card" : {
    "prefix" : "bs.card",
    "body" : [
        "<div class=\"card\">",
        "    <div class=\"card-header\">$0</div>",
        "    <div class=\"card-body\"></div>",
        "</div>",
    ],
    "description": "Add a col element."
},

"bootstrap col" : {
    "prefix" : "bs.col",
    "body" : [
        "<div class=\"col\">$0</div>",
    ],
    "description": "Add a col element."
},

"bootstrap row" : {
    "prefix" : "bs.row",
    "body" : [
        "<div class=\"row\">",
        "    <div class=\"col\">$0</div>",
        "</div>",
    ],
    "description": "Add a row element."
},

"h2 icon" : {
    "prefix" : "h2 icon",
    "body" : [
        "<h2 class=\"has-icon\">",
        "    <span class=\"icon\">",
        "        <i class=\"fas fa-save\"></i>",
        "    </span>",
        "    <span>$0</span>",
        "</button>",
    ],
    "description": "Add a h2 element."
},
```
