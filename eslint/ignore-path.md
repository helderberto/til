[back]: https://github.com/helderburato/til/tree/main/eslint

# `--ignore-path`

With this parameter I can avoid duplicate the `.gitignore` to `.eslintignore`.

## Use Cases

Let's update a common `package.json` adding the `lint` such as:

```json
{
  "scripts": {
    "lint": "eslint --ignore-path .gitignore ."
  }
}
```

Notice I'm passing the `eslint --ignore-path .gitignore .` it will uses the project root `.gitignore` to avoid validate unnecessary files and folders.

---

[← Back][back]
