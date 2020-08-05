```json
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
