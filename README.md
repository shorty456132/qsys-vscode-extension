# Q-SYS VSCode Extension

## Overview
`qsys-vscode-extension` is an extension for Visual Studio Code designed specifically for Q-SYS plugin development. It provides IntelliSense support and a set of snippets tailored for the Q-SYS Basic Plugin Framework, streamlining the plugin creation process.

## Features
- **IntelliSense Integration**: Enhances coding efficiency with Q-SYS plugin development by offering IntelliSense support.
- **Code Snippets**: A collection of snippets that can be inserted using keywords, speeding up the coding process.
- **Version 1.0.1**: Continuously evolving with the community's contributions.

## Getting Started
This extension is designed to be intuitive for users familiar with Q-SYS and VS Code. Simply type in the provided keywords to trigger IntelliSense and insert code blocks.

### Installation
Install the extension directly from the Visual Studio Code Marketplace.

## Snippets and Keywords
The extension includes several snippets that can be accessed using specific keywords:

### Controls (`ctrl` or `controls`)
Automatically generates a controls code block. Further properties can be added after the initial insertion.
```lua
table.insert(ctrls, {
  Name = "",
  Count = 1,
  ControlType = "Button | Indicator | Knob | Text"
})
```

### Properties (`props` or `properties`)
Builds out the table insertion for properties, focusing on the most commonly used ones.

### Graphics (`graphics`)
Adds entries to the `controlLayouts` table.

### Layout (`layout`)
Inserts layout configurations into the `layout` table with commonly used properties.

### Individual Keywords
- **HTextAlign**: Aligns text horizontally.
- **Position**: Sets the position of an element.
- **Size**: Defines the size of an element.
- **ButtonType**: Sets the type of a button control.
- **IndicatorType**: Specifies the type of an indicator.
- **UserPin**: Configures user pins.
- **PinStyle**: Determines the pin style.

## Contributing
This project is open to public contributions. Feel free to add new features, improve existing ones, or suggest changes. Your input is valuable in making this tool more effective for everyone.

## License
This extension is released under an open-source license, inviting widespread collaboration and modification.

## Notes
- Ensure you are familiar with the Q-SYS Basic Plugin Framework for effective use of this extension.
- This extension is in active development; stay tuned for more updates and features.
