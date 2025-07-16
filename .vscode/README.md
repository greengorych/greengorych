# VS Code Project Settings

This README explains the Visual Studio Code settings used in this project.

The `.vscode/settings.json` file keeps formatting, indentation, and file endings consistent across the project to reduce diffs and keep the code clean.

```json
{
  "editor.detectIndentation": false,
  "editor.formatOnSave": true,
  "editor.insertSpaces": true,
  "editor.tabSize": 2,
  "files.eol": "\n",
  "files.trimTrailingWhitespace": true,
  "files.insertFinalNewline": true,
  "files.trimFinalNewlines": true,
  "[json]": {
    "editor.tabSize": 2,
    "editor.insertSpaces": true
  },
  "[markdown]": {
    "editor.tabSize": 2,
    "editor.insertSpaces": true,
    "editor.wordWrap": "on"
  }
}

```

## Explanation:

- `"editor.detectIndentation": false` – always use the configured indentation instead of guessing from file content.
- `"editor.formatOnSave": true` – automatically format supported files on save.
- `"editor.insertSpaces": true` – use spaces instead of hard tab characters.
- `"editor.tabSize": 2` – default indentation size: 2 spaces.
- `"files.eol": "\n"` – enforce Unix-style LF line endings for consistency across platforms.
- `"files.trimTrailingWhitespace": true` – remove trailing whitespace on save.
- `"files.insertFinalNewline": true` – ensure each file ends with a single newline.
- `"files.trimFinalNewlines": true` – remove extra blank lines at the end of files.
- `"editor.wordWrap": "on"` - wrap long text lines automatically for better readability.
- `"[json]"` and `"[markdown]"` – explicit definitions of editor settings for these languages to ensure a consistent formatting style and behavior.

## Purpose:

By including these settings, all contributors get a consistent editing experience, preventing unexpected formatting changes or diffs.
