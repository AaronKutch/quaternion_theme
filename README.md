# Quaternion Color theme

Designed with the Rust programming language in mind, but should work with many other languages.

Note: in order for this theme to work properly, I highly recommend that you copy the following into
your VScode settings.json (open Settings and find the small icon in the upper right with the
description "Open Settings (JSON)"):
```text
    "editor.bracketPairColorization.enabled": true,
    "editor.guides.bracketPairs": true,
    "editor.bracketPairColorization.independentColorPoolPerBracketType": true,
    "workbench.colorCustomizations": {
        "editorBracketHighlight.foreground1": "#c49d00",
        "editorBracketHighlight.foreground2": "#ff8080",
        "editorBracketHighlight.foreground3": "#ff2adc",
        "editorBracketHighlight.foreground4": "#a35bff",
        "editorBracketHighlight.foreground5": "#00b2ff",
        "editorBracketHighlight.foreground6": "#00cb9d",
        "editorBracketHighlight.unexpectedBracket.foreground": "#f00",
    },
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

    // If the font turns into some nonmonospace font it has not been installed correctly
    "editor.fontFamily": "Input Regular",
    "debug.console.fontFamily": "Input Regular",
    // you may need to adjust this for your display so
    // that the aliasing falls on the right boundaries
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

    // Sometimes it is faster to do without
    //"editor.autoClosingComments": "never",
    //"editor.autoClosingQuotes": "never",

    // Important for rust-analyzer to not conflict with your manual builds
    "rust-analyzer.cargo.targetDir": true,
```

Important colors used:
```text
#a0a0a0 (stop things from interpreting as issue numbers)
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
