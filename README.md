# vscode
vscode config file

# windows settings path:
`C:\Users\user_name\AppData\Roaming\Code\User`

# extensions used:
```
Github Light Monochrome
Zenburn
Python
Python Docstring Generator
C/C++
Code Spell Checker
Matlab
matlab-formatter
PowerShell
LaTeX Workshop
Markdown All in One
Live Share
GitLens
```

# settings
```
{
    // telemetry
    "telemetry.enableCrashReporter": false,
    "telemetry.enableTelemetry": false,
    // common
    "editor.rulers": [
        79,
        120
    ],
    "editor.fontSize": 15,
    "editor.fontFamily": "JetBrains Mono",
    "terminal.integrated.fontSize": 15,
    "debug.console.fontSize": 15,
    "editor.cursorBlinking": "solid",
    "workbench.colorTheme": "Sublime Text 4 Theme",
    "editor.wordWrapColumn": 120,
    //
    "files.autoSave": "afterDelay",
    "files.autoSaveDelay": 30000,
    "files.trimTrailingWhitespace": true,
    "editor.cursorStyle": "block",
    // python
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
    "notebook.lineNumbers": "on",
    "python.linting.flake8Enabled": true,
    "python.linting.pylintEnabled": false,
    "python.linting.pydocstyleEnabled": true,
    "python.linting.flake8Args": [
        "--ignore=E203,W503,E501"
    ],
    "python.linting.flake8CategorySeverity.E": "Information",
    // markdown
    "[markdown]": {
        "editor.defaultFormatter": "yzhang.markdown-all-in-one"
    },
    // completion and spellcheck
    "cSpell.enabled": true,
    // "editor.quickSuggestions": false,
    // "editor.parameterHints.enabled": false,
    // "editor.suggestOnTriggerCharacters": false,
    "editor.acceptSuggestionOnEnter": "off",
    // visual settings/random
    "editor.folding": false,
    "editor.renderLineHighlight": "all",
    "editor.minimap.enabled": false,
    "workbench.editor.tabCloseButton": "off",
    "workbench.tree.indent": 14,
    "workbench.sideBar.location": "right",
    "window.enableMenuBarMnemonics": false,
    // git lens
    "gitlens.codeLens.enabled": false,
    "gitlens.currentLine.enabled": false,
    // latex workshop
    "[latex]": {
        "editor.wordWrap":"wordWrapColumn"
    },
    "latex-workshop.latex.recipe.default": "lastUsed",
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
            "name": "latexmk_rconly",
            "command": "latexmk",
            "args": [
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
            "name": "bibtex",
            "command": "bibtex",
            "args": [
                "%DOCFILE%"
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
        {
            "name": "rnw2tex",
            "command": "Rscript",
            "args": [
                "-e",
                "knitr::opts_knit$set(concordance = TRUE); knitr::knit('%DOCFILE_EXT%')"
            ],
            "env": {}
        },
        {
            "name": "jnw2tex",
            "command": "julia",
            "args": [
                "-e",
                "using Weave; weave(\"%DOC_EXT%\", doctype=\"tex\")"
            ],
            "env": {}
        },
        {
            "name": "jnw2texmintex",
            "command": "julia",
            "args": [
                "-e",
                "using Weave; weave(\"%DOC_EXT%\", doctype=\"texminted\")"
            ],
            "env": {}
        },
        {
            "name": "tectonic",
            "command": "tectonic",
            "args": [
                "--synctex",
                "--keep-logs",
                "%DOC%.tex"
            ],
            "env": {}
        }
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

        {
            "name": "latexmk 🔃",
            "tools": [
                "latexmk"
            ]
        },
        {
            "name": "latexmk (latexmkrc)",
            "tools": [
                "latexmk_rconly"
            ]
        },
        {
            "name": "latexmk (lualatex)",
            "tools": [
                "lualatexmk"
            ]
        },
        {
            "name": "pdflatex ➞ bibtex ➞ pdflatex × 2",
            "tools": [
                "pdflatex",
                "bibtex",
                "pdflatex",
                "pdflatex"
            ]
        },
        {
            "name": "Compile Rnw files",
            "tools": [
                "rnw2tex",
                "latexmk"
            ]
        },
        {
            "name": "Compile Jnw files",
            "tools": [
                "jnw2tex",
                "latexmk"
            ]
        },
        {
            "name": "tectonic",
            "tools": [
                "tectonic"
            ]
        }
    ],

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