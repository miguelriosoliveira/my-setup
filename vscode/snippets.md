```json
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
