# vscode
vscode config file

# windows settings path: 
`C:\Users\user_name\AppData\Roaming\Code\User`

# extensions used:
```
Github Light Monochrome
Monochrome dark
Find-Jump
Python
C/C++
Code Spell Checker
Matlab
matlab-formatter
PowerShell
Live Share
```

# settings
```
{
    "telemetry.enableCrashReporter": false,
    "telemetry.enableTelemetry": false,
    
    "editor.rulers": [
        80,
        120
    ],
    "editor.fontSize": 17,
    "terminal.integrated.fontSize": 17,
    "debug.console.fontSize": 17,
    "editor.cursorStyle": "block",
    "editor.cursorBlinking": "solid",
    "workbench.colorTheme": "Monochrome Dark",

    "python.venvPath": "C:\\Users\\user_name\\venv",
    "python.formatting.provider": "black",
    "python.analysis.autoImportCompletions": false,
    "workbench.editorAssociations": {
        "*.ipynb": "jupyter.notebook.ipynb"
    },

    "cSpell.enabled": false,
    "editor.quickSuggestions": false,
    "editor.acceptSuggestionOnEnter": "off",
    "editor.parameterHints.enabled": false,
    "editor.suggestOnTriggerCharacters": false,

    "editor.folding": false,
    "breadcrumbs.enabled": false,
    "breadcrumbs.icons": false,
    "editor.colorDecorators": false,
    "editor.find.addExtraSpaceOnTop": false,
    "editor.links": false,
    "editor.occurrencesHighlight": false,
    "editor.renderLineHighlight": "all",
    "editor.renderWhitespace": "none",
    "editor.roundedSelection": false,
    "editor.selectionHighlight": false,
    "workbench.editor.showIcons": false,
    "workbench.editor.tabCloseButton": "off",
    "workbench.iconTheme": null,
    "workbench.tree.indent": 14,
    "workbench.tree.renderIndentGuides": "none",
    "editor.lineNumbers": "off",
    "workbench.sideBar.location": "right",
    "window.enableMenuBarMnemonics": false,
}
```

# keybindings
```
// Place your key bindings in this file to override the defaultsauto[]
[
	{
		"key": "alt+s",
		"command": "findJump.activate"
	},
	{
		"key": "f1",
		"command": "-workbench.action.showCommands"
	},
	{
		"key": "f1",
		"command": "workbench.action.quickOpenTerm"
	},
	{
		"key": "alt+m",
		"command": "workbench.action.toggleMaximizedPanel"
	},
	{
		"key": "alt+f",
		"command": "search.action.openNewEditor"
	},
	
	{
		"key": "ctrl+down",
		"command": "cursorMove",
		"when": "editorTextFocus", 
		"args": {
			"to": "nextBlankLine",
			"by": "wrappedLine"
		}
	},
	{
		"key": "ctrl+up",
		"command": "cursorMove",
		"when": "editorTextFocus", 
		"args": {
			"to": "prevBlankLine",
			"by": "wrappedLine"
		}
	}
]
```