# vscode
vscode config file

# windows settings path:
`C:\Users\user_name\AppData\Roaming\Code\User`

# extensions used:
```
Python
Python Docstring Generator
Language-Cython
C/C++
Code Spell Checker
Matlab
LaTeX Workshop
<<<<<<< HEAD
Live Share
GitLens
Git Graph
Diff
Dracula
=======
Markdown All in One
GitLens
Git Graph
Diff
Zenburn optimized
>>>>>>> b9fb8e7 (update config)
```

# settings
```
{
    // telemetry
    "telemetry.telemetryLevel": "off",
    // common
    "editor.rulers": [
        79,
        120
    ],
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
    //
    "autoDocstring.docstringFormat": "sphinx-notypes",
    "python.venvPath": "~/venv",
    "python.analysis.autoImportCompletions": false,
    "workbench.editorAssociations": {
        "*.ipynb": "jupyter-notebook",
        "*.pdf": "latex-workshop-pdf-hook"
    },
    "notebook.lineNumbers": "on",
    "python.linting.flake8Args": [
        "--ignore=E203,W503,E501"
    ],
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
    "editor.bracketPairColorization.independentColorPoolPerBracketType": true,
    "git.openRepositoryInParentFolders": "never",
    "editor.minimap.enabled": false,
    "terminal.integrated.persistentSessionReviveProcess": "never",
    "terminal.integrated.enablePersistentSessions": false,
    "editor.fontFamily": "Jetbrains Mono",
    "editor.fontSize": 15,
}
```

# keybindings
```
[
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
		"key": "alt+h",
		"command": "editor.action.showHover",
		"when": "editorTextFocus"
	},
	{
		"key": "ctrl+k ctrl+i",
		"command": "-editor.action.showHover",
		"when": "editorTextFocus"
	},
]
```