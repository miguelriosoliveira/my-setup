# User Settings (Work)

```json
{
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.fontFamily": "Fira Code",
  "editor.fontLigatures": true,
  "editor.formatOnSave": true,
  "editor.rulers": [120],
  "editor.tabSize": 2,

  "files.autoSave": "onFocusChange",
  "files.exclude": {
    "**/.vscode/": true,
    "**/build/": true,
    "**/lib/": true,
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

  "terminal.integrated.rendererType": "dom",
  "terminal.integrated.shell.linux": "/bin/zsh",

  "window.titleBarStyle": "custom",

  "workbench.colorTheme": "Dracula",
  "workbench.editor.tabSizing": "shrink",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.startupEditor": "none",
}
```

# Keybidings (Work)

```json
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
  },
  {
    "key": "ctrl+shift+=",
    "command": "editor.unfoldAll",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "ctrl+k ctrl+j",
    "command": "-editor.unfoldAll",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "ctrl+shift+-",
    "command": "editor.foldAll",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "ctrl+k ctrl+0",
    "command": "-editor.foldAll",
    "when": "editorTextFocus && foldingEnabled"
  }
]
```
