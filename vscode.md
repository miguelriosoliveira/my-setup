# User Settings (Work)
```javascript
{
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.fontSize": 12,
  "editor.formatOnSave": true,
  "editor.rulers": [120],
  "editor.tabSize": 2,

  "files.autoSave": "onFocusChange",
  "files.exclude": {
    "**/.vscode/": true,
    "**/build/": true,
    "**/dist/": true,
    "**/node_modules/": true,
    "**/.idea/": true,
    "**/yarn-error.log": true
  },
  "files.trimTrailingWhitespace": true,
  "files.watcherExclude": {
    "**/.git/objects/**": true,
    "**/.git/subtree-cache/**": true,
    "**/node_modules/*/**": true
  },

  "git.autofetch": true,

  "gitlens.views.repositories.files.layout": "list",

  "javascript.implicitProjectConfig.experimentalDecorators": true,
  "javascript.updateImportsOnFileMove.enabled": "always",

  "prettier.eslintIntegration": true,

  "terminal.integrated.fontSize": 12,
  "terminal.integrated.shell.linux": "/bin/bash",

  "window.titleBarStyle": "custom",
  "window.zoomLevel": 0,

  "workbench.editor.tabSizing": "shrink",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.startupEditor": "none"
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
  {
    "key": "alt+1",
    "command": "workbench.action.toggleSidebarVisibility"
  },
  {
    "key": "ctrl+b",
    "command": "-workbench.action.toggleSidebarVisibility"
  }
]
```
