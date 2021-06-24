[back]: https://github.com/helderburato/til/tree/main/prettier

# `--ignore-path`

With this parameter I can avoid duplicate the `.gitignore` to `.eslintignore`.

## Use Cases

Let's update a common `package.json` adding the `lint` such as:

```json
{
  "scripts": {
    "format": "prettier --ignore-path .gitignore  \"**/*.+(js|json)\""
  }
}
```

Notice I'm passing the `prettier --ignore-path .gitignore` it will uses the project root `.gitignore` to avoid validate unnecessary files and folders.

And, the second part will ensure just files with extensions `js` or `json` will be formatted.

---

[← Back][back]
