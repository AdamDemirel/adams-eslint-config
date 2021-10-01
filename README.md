# adams-eslint-config
- My favourite ESlint rules

# Usage
In eslintrc file of project:
- `"extends": "adam-demirel"` or "eslint-config-adam-demirel" for standard JS linting rules
- `"extends": "adam-demirel/react"` or "eslint-config-adam-demirel/react for react linting rules

Example `.eslintrc.js`:
```js
module.exports = {
  env: {
    browser: true,
    es2021: true,
  },
  extends: [
    'adam-demirel',
  ],
  parserOptions: {
    ecmaVersion: 12,
    sourceType: 'module',
  },
};
```

# Recommended VScode settings
1. In CLI: `$ code --install-extension dbaeumer.vscode-eslint` to install `dbaeumer.vscode-eslint` extension (make sure it's enabled)

2. In VScodes `settings.json` (cmd+p + "Preferences: Open Settings (JSON)"):
```json
"editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
  },
"[javascript]": {
    "editor.defaultFormatter": "dbaeumer.vscode-eslint"
 },
```
- This formats linting rules on save
