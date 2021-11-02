# Quaternion Color theme

Designed with the Rust programming language in mind, but should work with many other languages.

Note: in order for this theme to work properly, I highly recommend that you use the Bracket Pair
Colorizer 2 extension (coenraads.bracket-pair-colorizer-2) and copy the following into your VScode
settings.json (open Settings and find "Open Settings (JSON)" in the upper right):
```text
    "bracket-pair-colorizer-2.colors": [
        "#c49d00",
        "#ff8080",
        "#ff2adc",
        "#a35bff",
    ],
```

Other things I recommend are the Error Lens extension (usernamehw.errorlens), the Input font face
(https://input.djr.com/, Input Mono size-14px Narrow Light lineheight-1x and default letterforms)
and these other settings for settings.json:
```text
    "workbench.colorTheme": "Quaternion",
    "workbench.colorCustomizations": {
        "[Quaternion]": {
            "editor.background": "#171717" // e.x. for if you want to customize further
        }
    },

    // If the font turns to some nonmonospace font it has not been installed correctly
    "editor.fontFamily": "Input Regular",
    "debug.console.fontFamily": "Input Regular",
    // may need to adjust this so the aliasing falls on the right boundaries
    "editor.fontSize": 14,

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

    // note: you might not want this if you do not have a source controlled environment
    "files.autoSave": "onFocusChange",
    "files.eol": "\n",
```

Important colors used:
```text
#RRGGBB CIELAB(L, A, B) color: use
#171717 (7.74, 0, 0) eigengrau: background
#777777 (50, 0, 0) gray: comments
#a0a0a0 (66, 0, 0) gray-white: variables
#00b2ff (66, 0, -128) blue: keywords
#00cb9d (66, -128, 0) cyan: types, strings
#2ab90f (66, -64, 64) green: constants, string punctuation
#c49d00 (66, 0, 128) yellow: punctuation
#ff8080 (68, 48, 23) peach: functions
#ff2adc (66, 96, -32) magenta: other
#a35bff (66, 96, -128) purple: other
```
