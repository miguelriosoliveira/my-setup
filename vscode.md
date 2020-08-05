# Settings

`settings.json`

```js
{
  "[css]": { "editor.defaultFormatter": "esbenp.prettier-vscode" },
  "[less]": { "editor.defaultFormatter": "esbenp.prettier-vscode" },
  "editor.codeActionsOnSave": { "source.fixAll": true },
  "editor.detectIndentation": false,
  "editor.fontFamily": "Fira Code",
  "editor.fontLigatures": true,
  "editor.fontSize": 13,
  "editor.formatOnSave": true,
  "editor.minimap.enabled": false,
  "editor.renameOnType": true,
  "editor.rulers": [100],
  "editor.tabSize": 2,

  "emmet.includeLanguages": { "javascript": "javascriptreact" },
  "emmet.syntaxProfiles": { "javascript": "jsx" },

  "eslint.enable": true,
  "eslint.packageManager": "yarn",

  "explorer.compactFolders": false,

  "files.associations": {
    ".zsh_aliases.*": "shellscript",
    ".prettierrc": "json"
  },
  "files.autoSave": "onFocusChange",
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

  "material-icon-theme.activeIconPack": "react",
  "material-icon-theme.files.associations": {
    "ormconfig.json": "database",
    "tsconfig.json": "tune"
  },
  "material-icon-theme.folders.associations": {
    "infra": "app",
    "entities": "class",
    "schemas": "class",
    "typeorm": "database",
    "repositories": "mappings",
    "http": "container",
    "migrations": "tools",
    "modules": "components",
    "implementations": "core",
    "dtos": "typescript",
    "fakes": "mock",
    "websockets": "pipe",
    "protos": "pipe",
    "grpc": "pipe"
  },

  "search.exclude": {
    "**/build/": true,
    "**/dist/": true,
    "**/lib": true,
    "**/node_modules": true
  },

  "terminal.integrated.fontSize": 12,
  "terminal.integrated.shell.linux": "/bin/zsh",

  "typescript.updateImportsOnFileMove.enabled": "always",

  "update.mode": "none",

  "window.titleBarStyle": "custom",

  "workbench.colorTheme": "Omni",
  "workbench.editor.labelFormat": "short",
  "workbench.editor.tabSizing": "shrink",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.sideBar.location": "right",
  "workbench.startupEditor": "none"
}
```

# Keybidings

`keybidings.json`

```json
[
  {
    "key": "ctrl+'",
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
  },
  {
    "key": "ctrl+alt+l",
    "command": "editor.action.transformToLowercase"
  },
  {
    "key": "ctrl+shift+o",
    "command": "workbench.action.openWorkspace"
  },
  {
    "key": "ctrl+shift+o",
    "command": "-workbench.action.gotoSymbol"
  }
]
```

# Snippets
```js
{
  "TypeScript functional component": {
    "prefix": "tsfc",
    "body": [
      "import React from 'react';",
      "",
      "const ${1:${TM_FILENAME_BASE}}: React.FC = () => {",
      "	return <div>${2:body}</div>;",
      "};",
      "",
      "export default ${1:${TM_FILENAME_BASE}};",
      ""
    ],
    "description": "TypeScript functional component"
  }
}

```
