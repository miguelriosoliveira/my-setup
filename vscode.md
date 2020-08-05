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
  // Place your global snippets here. Each snippet is defined under a snippet name and has a scope, prefix, body and
  // description. Add comma separated ids of the languages where the snippet is applicable in the scope field. If scope
  // is left empty or omitted, the snippet gets applied to all languages. The prefix is what is
  // used to trigger the snippet and the body will be expanded and inserted. Possible variables are:
  // $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders.
  // Placeholders with the same ids are connected.
  // Example:
  // "Print to console": {
  // 	"scope": "javascript,typescript",
  // 	"prefix": "log",
  // 	"body": [
  // 		"console.log('$1');",
  // 		"$2"
  // 	],
  // 	"description": "Log output to console"
  // }
  "Action": {
    "prefix": "rcac",
    "body": [
      "import alt from '@alt';",
      "import api from '@api';",
      "import sources from '@sources';",
      "",
      "class ${1:ComponentName}Actions {",
      "  get${1:ComponentName}(name) {",
      "    return async dispatch => {",
      "      let response = null;",
      "",
      "      try {",
      "        response = await api.get(sources.SOURCE_HERE, { params: { name } });",
      "      } catch (error) {",
      "        throw error;",
      "      }",
      "",
      "      dispatch(response.data);",
      "    };",
      "  }",
      "}",
      "",
      "export default alt.createActions(${1:ComponentName}Actions);",
      ""
    ],
    "description": "Action"
  },
  "Store": {
    "prefix": "rcst",
    "body": [
      "import alt from '@alt';",
      "",
      "import ${1:ComponentName}Actions from './${1:ComponentName}Actions';",
      "",
      "class ${1:ComponentName}Store {",
      "  constructor() {",
      "    this.bindActions(${1:ComponentName}Actions);",
      "  }",
      "}",
      "",
      "export default alt.createStore(${1:ComponentName}Store, '${1:ComponentName}Store');",
      ""
    ],
    "description": "Store"
  },
  "Component": {
    "prefix": "rccomp",
    "body": [
      "import React, { useEffect, useState } from 'react';",
      "",
      "import connectToStores from 'alt-utils/lib/connectToStores';",
      "",
      "import alt from '@alt';",
      "import GlobalActions from '@global/GlobalActions';",
      "import { getErrorMessage } from '@utils/utils';",
      "",
      "import ${1:ComponentName}Actions from './${1:ComponentName}Actions';",
      "import ${1:ComponentName}Store from './${1:ComponentName}Store';",
      "",
      "function ${1:ComponentName}({ history }) {",
      "  const [loading, setLoading] = useState(true);",
      "",
      "  // Similar to componentDidMount",
      "  useEffect(() => {",
      "    get${1:ComponentName}();",
      "    return () => alt.recycle(${1:ComponentName}Store);",
      "  }, []);",
      "",
      "  async function get${1:ComponentName}() {",
      "    setLoading(true);",
      "    try {",
      "      await ${1:ComponentName}Actions.get${1:ComponentName}();",
      "    } catch (error) {",
      "      GlobalActions.showMessage(getErrorMessage(error, '- DEFAULT ERROR MESSAGE HERE -'), 'error');",
      "    }",
      "    setLoading(false);",
      "  }",
      "",
      "  return <div></div>;",
      "}",
      "",
      "export default connectToStores(",
      "  {",
      "    getStores: () => [${1:ComponentName}Store],",
      "    getPropsFromStores: () => ${1:ComponentName}Store.getState(),",
      "  },",
      "  ${1:ComponentName},",
      ");",
      ""
    ],
    "description": "Component"
  }
}
```
