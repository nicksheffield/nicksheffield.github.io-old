---
title: "VIsual Studio Code Settings"
---

## User settings

{% highlight javascript %}
{
    "editor.fontFamily": "Hasklig",
    "editor.insertSpaces": false,
    "editor.fontLigatures": true,
    "workbench.colorTheme": "JetJet",
    "editor.lineHeight": 23,
    "editor.multiCursorModifier": "ctrlCmd",
    "editor.quickSuggestions": {
        "other": false,
        "comments": false,
        "strings": false
    },
    "files.exclude": {
        "**/.git": true,
        "**/.svn": true,
        "**/.hg": true,
        "**/CVS": true,
        "**/.DS_Store": true,
        "**/tmp": true,
        "**/tests": true
    },
    "editor.minimap.renderCharacters": false,
    "editor.parameterHints": false,
    "editor.mouseWheelZoom": true,
    "editor.renderWhitespace": "none",
    "window.zoomLevel": 0,
    "workbench.iconTheme": "seti",
    "git.confirmSync": false,
    "git.enableSmartCommit": true,
    "emmet.triggerExpansionOnTab": true
}
{% endhighlight %}

### Keybindings.json 
{% highlight javascript %}
// Place your key bindings in this file to overwrite the defaults
[
	{
		"key": "cmd+y",
		"command": "redo",
		"when": "editorTextFocus && !editorReadonly"
	},
	{
		"key": "shift+cmd+z",
		"command": "-redo",
		"when": "editorTextFocus && !editorReadonly"
	},
	{
		"key": "ctrl+tab",
		"command": "workbench.action.nextEditor"
	},
	{
		"key": "alt+cmd+right",
		"command": "-workbench.action.nextEditor"
	},
	{
		"key": "ctrl+shift+tab",
		"command": "workbench.action.previousEditor"
	},
	{
		"key": "alt+cmd+left",
		"command": "-workbench.action.previousEditor"
	},
	{
		"key": "shift+cmd+d",
		"command": "editor.action.copyLinesDownAction",
		"when": "editorTextFocus && !editorReadonly"
	},
	{
		"key": "shift+alt+down",
		"command": "-editor.action.copyLinesDownAction",
		"when": "editorTextFocus && !editorReadonly"
	}
]
{% endhighlight %}
