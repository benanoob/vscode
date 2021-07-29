# vscode
vscode config file

# windows settings path:
`C:\Users\user_name\AppData\Roaming\Code\User`

# extensions used:
```
Github Light Monochrome
Atom One Dark Theme
Find-Jump
Python
Python Docstring Generator
C/C++
Code Spell Checker
Matlab
matlab-formatter
PowerShell
LaTeX Workshop
Live Share
Format-Files
```

# settings
```
{
    "telemetry.enableCrashReporter": false,
    "telemetry.enableTelemetry": false,
    "editor.rulers": [
        79,
        120
    ],
    "editor.fontSize": 16,
    "editor.fontFamily": "JetBrains Mono",
    "terminal.integrated.fontSize": 16,
    "debug.console.fontSize": 16,
    "editor.cursorBlinking": "solid",
    "editor.cursorStyle": "block",
    "workbench.colorTheme": "Atom One Dark",


    "python.venvPath": "C:\\Users\\Eiosis\\venv",
    "python.formatting.provider": "black",
    "python.analysis.autoImportCompletions": false,
    "workbench.editorAssociations": {
        "*.ipynb": "jupyter-notebook"
    },
    "notebook.cellToolbarLocation": {
        "default": "right",
        "jupyter-notebook": "left"
    },
    "python.linting.flake8Enabled": true,
    "python.linting.pylintEnabled": false,
    "python.linting.pydocstyleEnabled": true,
    "python.linting.flake8Args": [
        "--ignore=E203,W503"
    ],
    "python.linting.flake8CategorySeverity.E": "Information",

    "[markdown]": {
        "editor.defaultFormatter": "yzhang.markdown-all-in-one"
    },

    "cSpell.enabled": false,
    // "editor.quickSuggestions": false,
    // "editor.parameterHints.enabled": false,
    // "editor.suggestOnTriggerCharacters": false,
    "editor.acceptSuggestionOnEnter": "off",
    "editor.suggestSelection": "first",
    "vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue",
    "breadcrumbs.enabled": false,
    "breadcrumbs.icons": false,
    "editor.folding": false,
    "editor.colorDecorators": false,
    "editor.find.addExtraSpaceOnTop": false,
    "editor.renderLineHighlight": "all",
    "editor.roundedSelection": false,
    "editor.lineNumbers": "off",
    "editor.renderIndentGuides": false,
    "editor.minimap.enabled": false,
    "notebook.lineNumbers": "on",
    "workbench.editor.showIcons": false,
    "workbench.editor.tabCloseButton": "off",
    "workbench.iconTheme": null,
    "workbench.tree.indent": 14,
    "workbench.sideBar.location": "right",
    "window.enableMenuBarMnemonics": false,

    "files.trimTrailingWhitespace": true,
}
```

# keybindings
```
// Place your key bindings in this file to override the defaultsauto[]
[
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
	},
	{
		"key": "ctrl+alt+b",
		"command": "markdown.extension.editing.toggleBold",
		"when": "editorTextFocus && !editorReadonly && editorLangId == 'markdown'"
	},
	{
		"key": "ctrl+b",
		"command": "-markdown.extension.editing.toggleBold",
		"when": "editorTextFocus && !editorReadonly && editorLangId == 'markdown'"
	},
	]
```