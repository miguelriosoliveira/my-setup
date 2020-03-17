# User Settings (Work)

```json
{
  "editor.codeActionsOnSave": {
    "source.fixAll": true
  },
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
  },
  {
    "key": "ctrl+alt+l",
    "command": "editor.action.transformToLowercase"
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
		  "import alt from '../../alt';",
		  "",
		  "import ${1:ComponentName}Source from './${1:ComponentName}Source';",
		  "",
		  "class ${1:ComponentName}Actions {",
		  "  basicFunction(name) {",
		  "    return async dispatch => {",
		  "      let response = null;",
		  "",
		  "      try {",
		  "        response = await ${1:ComponentName}Source.simpleGet();",
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
	  "Source": {
		"prefix": "rcsc",
		"body": [
		  "import api from '../../api';",
		  "import sources from '../../sources';",
		  "",
		  "export default class ${1:ComponentName}Source {",
		  "  static simpleGet(name) {",
		  "    return api.get(sources, { params: { name } });",
		  "  }",
		  "}",
		  ""
		],
		"description": "Source"
	  },
	  "Store": {
		"prefix": "rcst",
		"body": [
		  "import alt from '../../alt';",
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
	  }
}
```
