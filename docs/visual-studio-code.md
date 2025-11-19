# Visual Studio Code

## Shortcuts

| Shortcut      | Beschreibung |
| ----------- | ----------- |
| <kbd>CTRL</kbd>+<kbd>K</kbd> <kbd>V</kbd>       | Markdown Preview       |
|   <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd><br/>  Type: Preferences: Open Settings (JSON) |   settings.json öffnen      |
| <kbd>CTRL</kbd>+<kbd>C</kbd>       | Line Comment |
| <kbd>CTRL</kbd>+<kbd>U</kbd>       | Line Uncomment |
| <kbd>ALT</kbd>+<kbd>SHIFT</kbd>+<kbd>F</kbd>       | Format Code (Tastenreihenfolge beachten)|
| <kbd>CTRL</kbd>+<kbd>SHIFT</kbd>+<kbd>P</kbd>       | Command Palette |
| <kbd>CTRL</kbd>+<kbd>SHIFT</kbd>+<kbd>B</kbd>       | Run Build Task |
| <kbd>CTRL</kbd>+<kbd>,</kbd>       | Open Settings |
| <kbd>ALT</kbd>+<kbd>&larr;</kbd>       | last edited Position |
| <kbd>CTRL</kbd>+<kbd>K</kbd>+<kbd>L</kbd>       | Toggle Region |
| **Clipboard History** ||
| <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>V</kbd> <kbd>D</kbd>  | opens the clipboard delete settings. Use the arrow keys to scroll and press Enter to remove a selected item. |
| <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>V</kbd> <kbd>E</kbd> | opens the clipboard editor settings. Use the arrow keys to scroll and press Enter to edit a selected item.
| **vscode-pandoc** ||
| <kbd>Ctrl</kbd>+<kbd>K</kbd> <kbd>P</kbd>  | choose from the list what document type you want to render. |
es geht auch
| <kbd>F1</kbd> pandoc  | choose from the list what document type you want to render. |

## Extensions

* Clipboard - Digoro.clipboard
* OverType - DrMerfy.overtype
* YAML - redhat.vscode-yaml
* Debugger for Chrome
* markdownlint - DavidAnson.vscode-markdownlint
* React Extension Pack (ESLint, npm, ...)
* vscode-pandoc

## EsLint einrichten

```console
npm install eslint --save-dev
npm install eslint-plugin-disable --save-dev
npx eslint --init
```

Konfiguration in .eslintrc.json. Bsp:

```json
{
    // each environment provides predefined global variables
    "env": {
        // browser global variables such as 'name', 'self', 'top'
        "browser": true,
        // adds all ECMAScript 2021 globals and automatically sets the ecmaVersion parser option to 12
        "es2021": true
    },
    // npm packages that add various extensions to ESLint
    "plugins": [
        "react",
        "@typescript-eslint"
    ],
    // extends: merging extension-configs into the base configuration.
    // The eslint-config- prefix can be omitted from the configuration name.
    // Here we are merging the recommended Rules
    "extends": [
        "eslint:recommended",
        "plugin:react/recommended",
        "plugin:@typescript-eslint/recommended"
    ],
    // define custom parser
    "parser": "@typescript-eslint/parser",
    "parserOptions": {
        "sourceType": "module",
        "ecmaVersion": 2020,
        "ecmaFeatures": {
            "jsx": true
        }
    },

    // configurations that will only apply to files that match specific patterns
    "overrides": [
        // typescript
        {
          "files": ["*.ts", "*.tsx"]
        },
        {
            "files": ["**/.jsx", "**/*.js"],
            "settings": {
                "disable/plugins": ["@typescript-eslint"]
            }
            
        }    
  
    ],

    "rules": {
        // Section: enable additonal rules
        "no-console": "off"
        
        // Section modify recommended rules

        // Section disable rules from base configuration
    }
}
```

## Pandoc einrichten

In settings.json den Code-Block für die Wordausgabe konfigurieren, z.B.: `zenburn`, `tango` oder `breezedark`.

```json
{
    // ...
    "pandoc.docxOptString": "--highlight-style default"
}
```

## Redux Debugging

* Redux DevTools Extension für Chrome installieren.
* ```npm install --save-dev redux-devtools-extension```
* die Extension wird im ```configureStore``` des ReduxToolKits automatisch aktiviert.
