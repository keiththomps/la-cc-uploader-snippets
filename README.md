# la-cc-uploader-snippets

This package provides snippets for working creating flash cards and exam questions withing CC and LA.

## Installation

Download the extension to your extensions directory

```
cd ~/.vscode/extensions
git clone https://github.com/keiththomps/la-cc-uploader-snippets.git
```

You may not have snippet expansion enabled for YAML strings. If you don't see an expansion in a new YAML file when you type `que` then add the following to your settings JSON (You can type `Cmd+Shift+P` and search for "settings json" to get to this file):

```json
{
  // other settings
  "[yaml]": {
    "editor.quickSuggestions": {
      "other": true,
      "comments": false,
      "strings": true
    }
  }
}
```

## Usage

From within a YAML file you can run the following snippets

- `que` - Expands into a question item.
- `nno` - Expands to `None of these choices.`
- `oone` - Expands to `One of these choices is correct.`
- `aall` - Expands to `All of these choices.`
- `flash` - Expands into a flash card item.
