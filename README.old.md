# google-places-autocomplete

## Progress:

1. `npx create-react-app .`

2. `npm install --save-dev prettier eslint`

3. `npx mrm lint-staged`

4. Setting in `package.json`:

```
"lint-staged": {
    "*.{js,jsx}": "eslint --cache --fix",
    "*.{js,jsx,css,scss,md}": "prettier --write"
  }
```

5. Add `.prettirrc` in the root

6. Add `.huskyrc` in the root:

```
{
    "hooks": {
    "pre-commit": "lint-staged"
    }
}
```

7. Add `.lintstagedrc` in the root:

```
{
    "src/**/\*.{json,css,scss,md}": ["prettier --write"],
    "src/**/\*.{js,jsx,ts,tsx}": ["prettier --write", "eslint --fix"]
}
```

8. `npm run build`

9. Add `"homepage": "..."`

10. `npm run build`

11. `npm install --save gh-pages`

12. Add scripts in `package.json`:

```
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build"
```

13. `npm run deploy`

14. `npm install modern-normalize`  
    `npm install node-sass --save`

15. `npm install @material-ui/core`  
    `npm install @material-ui/icons`

16. Add code and icons to `App.jsx`

17.
