# vscode-twined-components

Syntax highlighting and IntelliSense for [twined-components](https://github.com/lowfront/twined-components)'s CSS code. It also works for classnames when used with [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss).

![Syntax highlighting in action](https://raw.githubusercontent.com/lowfront/vscode-twined-components/master/demo.png)

## Usage

The twined-components extension adds highlighting and IntelliSense for twined-component template strings in JavaScript and TypeScript.

## With Tailwind CSS IntelliSense
Setting the `experimental.classRegex` property of [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss) as below supports Syntax highlighting and IntelliSense for classnames.

```json
// settings.json
{
  ...
    "tailwindCSS.experimental.classRegex": [
      "twined.[a-z0-9]+?`([^`]*)",
      "twined\\(\\w+?\\)`([^`]*)",
    ]
  ...
}
```

### Caution
For `Tailwind CSS IntelliSense` to work, the `tailwind.config.js` file must be present at the project root directory. If it does not work, create `tailwind.config.js` as shown in the [document](https://tailwindcss.com/docs/configuration) and restart Extension Host (`Ctrl + p` > Developer: Restart Extension Host). Check [here](https://github.com/tailwindlabs/tailwindcss-intellisense#troubleshooting) for more information.