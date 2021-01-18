# vscode-twined-components

Syntax highlighting and IntelliSense for [twined-components](https://github.com/lowfront/twined-components)'s CSS code. It also works for classnames when used with [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss).

![Syntax highlighting in action](https://raw.githubusercontent.com/lowfront/vscode-twined-components/master/demo.png)

## Usage

The twined-components extension adds highlighting and IntelliSense for twined-component template strings in JavaScript and TypeScript.

## With tailwindcss-intellisense
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