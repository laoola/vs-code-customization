# VS Code Customization

This guide will help you customize your Visual Studio Code to use the GitHub Dark theme, JetBrains Mono font, and the "Custom CSS and JS Loader" extension with a custom CSS file.

![image](https://github.com/user-attachments/assets/a85a2168-a67d-4ab6-8cdd-b7a197e86aca)

## Prerequisites

- Visual Studio Code
- "Custom CSS and JS Loader" extension installed
- "GitHub Theme" theme

## Steps

### 2. Install JetBrains Mono Font

1. Download the JetBrains Mono font from the [official website](https://www.jetbrains.com/lp/mono/).
2. Install the font on your system.

### 3. Configure VS Code to Use JetBrains Mono

1. Open Visual Studio Code.
2. Go to `File > Preferences > Settings` or press `Ctrl+,`.
3. Search for "Font Family" and set it to `'JetBrains Mono', Consolas, 'Courier New', monospace`.

> Or edit the Settings JSON file:

```json
{
    "editor.fontFamily": "JetBrains Mono, Consolas, 'Courier New', monospace",
    "editor.fontSize": 13,
    "editor.fontLigatures": true
}
```

### 4. Use Custom CSS with "Custom CSS and JS Loader" Extension

1. Open Visual Studio Code.
2. Go to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window or by pressing `Ctrl+Shift+X`.
3. Search for "Custom CSS and JS Loader" and install it.
4. Create a CSS file with the following content and save it as `custom-vscode.css` in your preferred location:
5. Add Custom CSS to Settings

Add the following to your `settings.json`:

```json
"vscode_custom_css.imports": [
    // Absolute file paths for your css/js files
    // For Mac or Linux
    // "file:///Users/your-user-name/custom-vscode.css",
    // "file:///Users/your-user-name/custom-vscode-script.js"

    // For Windows
    // "file:///Drive:/path-of-custom-css/custom-vscode.css",
    // "file:///Drive:/path-of-custom-js/custom-vscode-script.js"
],
```

6. Open the Command Palette by pressing `Ctrl+Shift+P`.
7. Type and select `Custom CSS and JS: Enable`.
8. Restart Visual Studio Code.

> [!NOTE]
> After making any changes to your custom CSS or JS files, you need to reload them in Visual Studio Code:

1. Open the Command Palette by pressing `Ctrl+Shift+P`.
2. Type and select `Reload Custom CSS and JS`.
3. Restart Visual Studio Code to apply the changes.
