# User Settings (Work)
```javascript
{
  /* FILES */

  // Controls auto save of dirty files. Accepted values:  'off', 'afterDelay', 'onFocusChange' (editor loses focus), 'onWindowChange' (window loses focus). If set to 'afterDelay', you can configure the delay in 'files.autoSaveDelay'.
  "files.autoSave": "onFocusChange",
  // Configure glob patterns for excluding files and folders. For example, the files explorer decides which files and folders to show or hide based on this setting.
  "files.exclude": {
    "**/.vscode/": true,
    "**/build/": true,
    "**/dist/": true,
    "**/node_modules/": true,
    "**/yarn-error.log": true
  },
  "files.watcherExclude": {
    "**/.git/objects/**": true,
    "**/.git/subtree-cache/**": true,
    "**/node_modules/*/**": true
  },
  // When enabled, will trim trailing whitespace when saving a file.
  "files.trimTrailingWhitespace": true,

  /* EDITOR */

  // Render vertical rulers after a certain number of monospace characters. Use multiple values for multiple rulers. No rulers are drawn if array is empty
  "editor.rulers": [120],
  // The number of spaces a tab is equal to. This setting is overridden based on the file contents when `editor.detectIndentation` is on.
  "editor.tabSize": 2,
  // Format a file on save. A formatter must be available, the file must not be auto-saved, and editor must not be shutting down.
  "editor.formatOnSave": true,
  // Controls the font size in pixels.
  "editor.fontSize": 12,

  /* JAVASCRIPT */

  // Enable/disable 'experimentalDecorators' for JavaScript files that are not part of a project. Existing jsconfig.json or tsconfig.json files override this setting. Requires TypeScript >=2.3.1.
  "javascript.implicitProjectConfig.experimentalDecorators": true,
  // Enable/disable automatic updating of import paths when you rename or move a file in VS Code. Requires using TypeScript 2.9 or newer in the workspace.
  "javascript.updateImportsOnFileMove.enabled": "always",

  /* WORKBENCH */

  // Controls the sizing of editor tabs. Set to 'fit' to keep tabs always large enough to show the full editor label. Set to 'shrink' to allow tabs to get smaller when the available space is not enough to show all tabs at once.
  "workbench.editor.tabSizing": "shrink",
  // Controls which editor is shown at startup, if none is restored from the previous session. Select 'none' to start without an editor, 'welcomePage' to open the Welcome page (default), 'newUntitledFile' to open a new untitled file (only opening an empty workspace).
  "workbench.startupEditor": "none",
  // Specifies the icon theme used in the workbench or 'null' to not show any file icons.
  "workbench.iconTheme": "material-icon-theme",

  /* TERMINAL */

  // Controls the font size in pixels of the terminal.
  "terminal.integrated.fontSize": 12,
  // The path of the shell that the terminal uses on Linux. [Read more about configuring the shell](https://code.visualstudio.com/docs/editor/integrated-terminal#_configuration).
  "terminal.integrated.shell.linux": "/bin/bash",

  /* WINDOW */

  // Adjust the zoom level of the window. The original size is 0 and each increment above (e.g. 1) or below (e.g. -1) represents zooming 20% larger or smaller. You can also enter decimals to adjust the zoom level with a finer granularity.
  "window.zoomLevel": -1
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
  {
    "key": "alt+right",
    "command": "workbench.action.terminal.focusNextPane",
    "when": "terminalFocus"
  },
  {
    "key": "alt+left",
    "command": "workbench.action.terminal.focusPreviousPane",
    "when": "terminalFocus"
  },
  {
    "key": "ctrl+alt+u",
    "command": "editor.action.transformToUppercase"
  },
  {
    "key": "shift+alt+l",
    "command": "editor.action.sortLinesAscending"
  },
]
```
