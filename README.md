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
