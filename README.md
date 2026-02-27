# vscode
vscode config file

# windows settings path:
`C:\Users\user_name\AppData\Roaming\Code\User`

# extensions used:
```
Python
ruff
ty
Python Docstring Generator
Language-Cython
C/C++
Code Spell Checker
Matlab
LaTeX Workshop
Git Graph
Diff
pico8-ls
Kivy

GitLens
Pylint
```

# settings
```json
{
    // visual
    "editor.fontFamily": "aporetic sans mono", // "jetbrains mono" is dope too
    "editor.fontSize": 18,
    "terminal.integrated.fontSize": 16,
    "window.autoDetectColorScheme": true,
    "workbench.activityBar.location": "top", // gain space, open sidebar with keyboard
    // files
    "files.trimTrailingWhitespace": true,
    "files.exclude": {
        "**/.git": false
    },
    // completion and spellcheck
    "editor.acceptSuggestionOnEnter": "off",
    // windows
    "terminal.integrated.defaultProfile.windows": "Git Bash",
    "terminal.integrated.env.windows": {
        "PYTHONPATH": "."
    },
    // I had weird bugs with terminal recalls soo turn it off
    "terminal.integrated.persistentSessionReviveProcess": "never",
    "terminal.integrated.enablePersistentSessions": false,
    // python
    "ty.inlayHints.variableTypes": false,
    "ty.inlayHints.callArgumentNames": false,
    "pylint.args": [
        "--rcfile=~/shannon/pylintrc"
    ],
    "autoDocstring.docstringFormat": "sphinx-notypes",
    "python.venvPath": ".venv",
    "python.analysis.autoImportCompletions": false,
    "workbench.editorAssociations": {
        "*.ipynb": "jupyter-notebook",
        "*.pdf": "latex-workshop-pdf-hook"
    },
    "notebook.lineNumbers": "on",
    // disable annoying stuff
    "chat.disableAIFeatures": true,
    "telemetry.telemetryLevel": "off",
    "editor.folding": false,
    "editor.minimap.enabled": false,
    "update.showReleaseNotes": false,
    "workbench.startupEditor": "none",
    "workbench.editor.enablePreview": false,
    "editor.occurrencesHighlight": "off",
    "MATLAB.showFeatureNotAvailableError": false,
    // latex workshop
    "[latex]": {
        "editor.wordWrap": "on"
    },
    "latex-workshop.view.pdf.viewer": "tab",
    // "latex-workshop.latex.autoBuild.run": "never",
    "latex-workshop.latex.tools": [
        {
            "name": "latexmk",
            "command": "latexmk",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-pdf",
                "-outdir=%OUTDIR%",
                "%DOC%"
            ],
            "env": {}
        },
        {
            "name": "lualatexmk",
            "command": "latexmk",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-lualatex",
                "-outdir=%OUTDIR%",
                "%DOC%"
            ],
            "env": {}
        },
        {
            "name": "pdflatex",
            "command": "pdflatex",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "%DOC%"
            ],
            "env": {}
        },
        {
            "name": "biber",
            "command": "biber",
            "args": [
                "%DOCFILE%"
            ],
            "env": {}
        },
    ],
    "latex-workshop.latex.recipes": [
        {
            "name": "pdflatex ➞ biber ➞ pdflatex × 2",
            "tools": [
                "pdflatex",
                "biber",
                "pdflatex",
                "pdflatex"
            ]
        },
    ],
}
```

# keybindings
```json
[
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
		"key": "f1",
		"command": "workbench.action.toggleSidebarVisibility"
	},
	{
		"key": "ctrl+b",
		"command": "-workbench.action.toggleSidebarVisibility"
	},
	{
		"key": "f3",
		"command": "workbench.action.terminal.toggleTerminal",
		"when": "terminal.active"
	},
	{
		"key": "ctrl+oem_3",
		"command": "-workbench.action.terminal.toggleTerminal",
		"when": "terminal.active"
	}
]
```