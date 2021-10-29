# Quaternion Color theme

Designed with the Rust programming language in mind, but should work with many other languages.

Note: in order for this theme to work properly, I highly recommend that you use the Bracket Pair
Colorizer 2 extension (coenraads.bracket-pair-colorizer-2) and copy the following into your VScode
settings.json (open Settings and find "Open Settings (JSON)" in the upper right):
```text
    "bracket-pair-colorizer-2.colors": [
        "#e0b500",
        "#ff8080",
        "#ff00be",
        "#b900ff",
    ],
```

Other things I recommend are the Error Lens extension (usernamehw.errorlens), the Input font face
(https://input.djr.com/, Input Mono size-14px Narrow Light lineheight-1x and default letterforms)
and these other settings for settings.json:
```text
    "workbench.colorTheme": "Quaternion",

    "editor.fontFamily": "Input Regular",
    "debug.console.fontFamily": "Input Regular",
    "editor.fontSize": 14, // may need to adjust this so the aliasing falls on the right boundaries

    "debug.console.wordWrap": true,
    "editor.minimap.renderCharacters": false,
    "editor.minimap.side": "left",
    "editor.minimap.maxColumn": 100,
    "editor.wordWrap": "bounded",
    "editor.rulers": [100], // if this is where maximum formatting width is
    "editor.cursorBlinking": "phase",
    "editor.cursorStyle": "block",
    "editor.wordWrapColumn": 120,
    "editor.renderWhitespace": "trailing",
    "workbench.colorCustomizations": {
        "[Quaternion]": {
            "editor.background": "#171717" // e.x. for if you want to customize further
        }
    },

    "files.autoSave": "onFocusChange",
    "files.eol": "\n",
```