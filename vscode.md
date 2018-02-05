# User Settings (Work)
```javascript
{
    // Controls the font size in pixels.
    "editor.fontSize": 12,
    // Render vertical rulers after a certain number of monospace characters. Use multiple values for multiple rulers. No rulers are drawn if array is empty
    "editor.rulers": [120],

    // Controls the font size in pixels of the terminal.
    "terminal.integrated.fontSize": 12,
    
    // Fit code within this line limit
    "prettier.printWidth": 120,
    // If true, will use single instead of double quotes
    "prettier.singleQuote": true,
    // Number of spaces it should use per tab
    "prettier.tabWidth": 4,

    // Controls which editor is shown at startup, if none is restored from the previous session. Select 'none' to start without an editor, 'welcomePage' to open the Welcome page (default), 'newUntitledFile' to open a new untitled file (only opening an empty workspace).
    "workbench.startupEditor": "none",
    // Specifies the icon theme used in the workbench or 'null' to not show any file icons.
    "workbench.iconTheme": "material-icon-theme"
}
```

# Keybidings (Work)
```javascript
// Place your key bindings in this file to overwrite the defaults
[
    {
        "key": "alt+8",
        "command": "workbench.action.terminal.toggleTerminal"
    },
    {
        "key": "shift+alt+down",
        "command": "editor.action.copyLinesDownAction",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "shift+alt+up",
        "command": "editor.action.copyLinesUpAction",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "ctrl+alt+s",
        "command": "importjs.fix",
        "when": "editorTextFocus"
    },
    {
        "key": "ctrl+shift+i",
        "command": "editor.action.formatDocument",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "ctrl+shift+i",
        "command": "-editor.action.formatDocument",
        "when": "editorTextFocus && !editorReadonly"
    },
]
```
