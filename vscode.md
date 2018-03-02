# User Settings (Work)
```javascript
{
    /*
    FILES
    */
    // Controls auto save of dirty files. Accepted values:  'off', 'afterDelay', 'onFocusChange' (editor loses focus), 'onWindowChange' (window loses focus). If set to 'afterDelay', you can configure the delay in 'files.autoSaveDelay'.
    "files.autoSave": "onFocusChange",
    // When enabled, will trim trailing whitespace when saving a file.
    "files.trimTrailingWhitespace": true,
    /*
    EDITOR
    */
    // Controls the font size in pixels.
    "editor.fontSize": 12,
    // Render vertical rulers after a certain number of monospace characters. Use multiple values for multiple rulers. No rulers are drawn if array is empty
    "editor.rulers": [
        120
    ],
    // The number of spaces a tab is equal to. This setting is overridden based on the file contents when `editor.detectIndentation` is on.
    "editor.tabSize": 2,
    // Format a file on save. A formatter must be available, the file must not be auto-saved, and editor must not be shutting down.
    "editor.formatOnSave": true,
    /*
    TERMINAL
    */
    // Controls the font size in pixels of the terminal.
    "terminal.integrated.fontSize": 12,
    /*
    PRETTIER
    */
    // Fit code within this line limit
    "prettier.printWidth": 120,
    // If true, will use single instead of double quotes
    "prettier.singleQuote": true,
    /*
    WORKBENCH
    */
    // Controls the sizing of editor tabs. Set to 'fit' to keep tabs always large enough to show the full editor label. Set to 'shrink' to allow tabs to get smaller when the available space is not enough to show all tabs at once.
    "workbench.editor.tabSizing": "shrink",
    // Controls which editor is shown at startup, if none is restored from the previous session. Select 'none' to start without an editor, 'welcomePage' to open the Welcome page (default), 'newUntitledFile' to open a new untitled file (only opening an empty workspace).
    "workbench.startupEditor": "none",
    // Specifies the icon theme used in the workbench or 'null' to not show any file icons.
    "workbench.iconTheme": "material-icon-theme",
}
```

# Keybidings (Work)
```javascript
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
        "key": "ctrl+shift+i",
        "command": "editor.action.formatDocument",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "ctrl+shift+i",
        "command": "-editor.action.formatDocument",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "alt+right",
        "command": "workbench.action.nextEditor"
    },
    {
        "key": "alt+left",
        "command": "workbench.action.previousEditor"
    },
]
```