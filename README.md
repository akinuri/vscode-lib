# vscode-lib

Collection of modifications to VS Code.

<br>

## Extensions

Keyboard Shortcut: `Ctrl + Shift + X`

* [Apache Conf](https://marketplace.visualstudio.com/items?itemName=mrmlnc.vscode-apache)
* [Favorites](https://marketplace.visualstudio.com/items?itemName=kdcro101.favorites)
* [GitLens — Git supercharged](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
* [Laravel Artisan](https://marketplace.visualstudio.com/items?itemName=ryannaddy.laravel-artisan)
* [Laravel Blade Snippets](https://marketplace.visualstudio.com/items?itemName=onecentlin.laravel-blade)
* [Laravel goto view](https://marketplace.visualstudio.com/items?itemName=codingyu.laravel-goto-view)
* [Live Sass Compiler](https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass)
* [Markdown Preview Enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)
* [PHP Intelephense](https://marketplace.visualstudio.com/items?itemName=bmewburn.vscode-intelephense-client)
* [PHP IntelliSense](https://marketplace.visualstudio.com/items?itemName=zobo.php-intellisense)
* [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
* [Selected Lines Count](https://marketplace.visualstudio.com/items?itemName=gurumukhi.selected-lines-count)
* [Sort lines](https://marketplace.visualstudio.com/items?itemName=Tyriar.sort-lines)
* [Sync Scroll](https://marketplace.visualstudio.com/items?itemName=dqisme.sync-scroll)
* [Todo Tree](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree)
* [Vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur)
* [php cs fixer](https://marketplace.visualstudio.com/items?itemName=junstyle.php-cs-fixer)
* [phpcs](https://marketplace.visualstudio.com/items?itemName=ikappas.phpcs)

<br>

## File > Preferences > Settings > Open Settings (JSON)

Keyboard Shortcut: `Ctrl + ,` `->` `Open Settings (JSON)`

```
"editor.fontSize": 13,
"editor.lineHeight": 20,
"editor.tabSize": 4,
"editor.insertSpaces": true,
"editor.trimAutoWhitespace": false,
"editor.snippetSuggestions" : "top",
"editor.autoIndent": "advanced",
"editor.bracketPairColorization.enabled": true,
"editor.renderControlCharacters": false,
"editor.minimap.enabled": false,
"editor.cursorBlinking": "phase",
"editor.smoothScrolling": true,
"editor.mouseWheelScrollSensitivity": 1.5,
"editor.fastScrollSensitivity": 3,
"editor.unicodeHighlight.allowedCharacters": {
	"ı": true
},
"editor.rulers": [
    80
],

"explorer.openEditors.visible": 0,

"workbench.tree.indent": 16,
"workbench.startupEditor": "newUntitledFile",
"workbench.colorTheme": "Visual Studio Light",

"php.suggest.basic": false,
"php.validate.executablePath": "C://xampp//php//php.exe",

"diffEditor.ignoreTrimWhitespace": false,

"window.zoomLevel": -1,

"todo-tree.general.tags": [
    "BUG",
    "HACK",
    "FIXME",
    "TODO",
    "XXX",
    "NOTE",
],
"todo-tree.filtering.excludeGlobs": [
    "**/assets/ext/**",
    "**/node_modules/**",
    "**/system/**",
    "**/vendor/**",
],
```

<br>

## File > Preferences > Keyboard Shortcuts

### Set

Keyboard Shortcut: `Ctrl + K Ctrl + S`

    Copy Line Down              -> Ctrl + D
    Toggle Line Comment         -> Ctrl + Q
    Toggle Block Comment        -> Ctrl + Alt + W
    Emmet: Go to Matching Pair  -> Ctrl + Alt + D
    Go to Bracket               -> Alt + D
    Fold All Regions            -> Ctrl + R
    Unfold All Regions          -> Alt + R

### Use

```
Fold All (Recursively)      -> Ctrl + K Ctrl + 0
Fold Level 1                -> Ctrl + K Ctrl + 1
Fold Level 2                -> Ctrl + K Ctrl + 2
Fold Level N                -> Ctrl + K Ctrl + N
Fold Recursively            -> Ctrl + K Ctrl + ğ
Fold All Regions            -> Ctrk + R             (previously Ctrl + K Ctrl + 8)
Fold All Regions Exc. Sele. -> Ctrk + K Ctrl + -

Unfold All                  -> Ctrl + K Ctrl + J
Unfold All Regions          -> Alt + R              (previously Ctrl + K Ctrl + 9)
```

<br>

## File > Preferences > [User Snippets](https://code.visualstudio.com/docs/editor/userdefinedsnippets)

Show snippets in editor: `Ctrl + Space`

### PHP

```
"Region Start (20 dashes)" : {
    "prefix"      : "#region20",
    "body"        : ["#region ==================== ${REGION}"],
    "description" : "Folding Region Start"
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
	
"Private Constructor" : {
    "prefix" : "__construct",
    "body" : [
    "private function __construct() {}",
    ],
    "description": "Private Class Constructor"
},
```

### JS

```
"Region Start (20 dashes)" : {
    "prefix" 	  : "#region20",
    "body" 		  : ["// #region ==================== ${REGION}"],
    "description" : "Folding Region Start"
},

"Region End (spaced)" : {
    "prefix"      : "#endregion",
    "body"        : ["// #endregion"],
    "description" : "Folding Region End"
},
```

### HTML

```
"comment" : {
    "prefix" : "comment",
    "body" : [
        "<!-- $0 -->",
    ],
    "description": "Add a comment."
},

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

"table" : {
    "prefix" : "table",
    "body" : [
        "<table>",
        "    <thead>",
        "        <tr>",
        "            <th>Header 1$0</th>",
        "            <th>Header 2</th>",
        "        </tr>",
        "    </thead>",
        "    <tbody>",
        "        <tr>",
        "            <td>Cell 1</td>",
        "            <td>Cell 2</td>",
        "        </tr>",
        "    </tbody>",
        "</table>",
    ],
    "description": "Add a table element."
},
```

### CSS

```
"Region Start (20 dashes)" : {
    "prefix"      : "#region20",
    "body"        : ["/* #region ==================== ${REGION} */"],
    "description" : "Folding Region Start"
},
```

### Python

```
"Region Start (20 dashes)" : {
    "prefix"      : "#region20",
    "body"        : ["#region ==================== ${REGION}"],
    "description" : "Folding Region Start"
},

"Region End" : {
    "prefix"      : "#endregion",
    "body"        : ["#endregion"],
    "description" : "Folding Region End"
},
```

