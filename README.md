# Q-SYS VSCode Extension

## Overview
`qsys-vscode-extension` is an extension for Visual Studio Code designed specifically for Q-SYS plugin development. It provides IntelliSense support and a set of snippets tailored for the Q-SYS Basic Plugin Framework, streamlining the plugin creation process.

## Features
- **IntelliSense Integration**: Enhances coding efficiency with Q-SYS plugin development by offering IntelliSense support.
- **Code Snippets**: A collection of snippets that can be inserted using keywords, speeding up the coding process.
- **Version 1.0.1**: Continuously evolving with the community's contributions.

<<<<<<< HEAD
<details>
 <summary><b>Version 1.1.0</b></summary>
  - Added Comment and Header for optional strings on properties
  - Added ButtonType  On, Off , Custom, StateTrigger
  - Added TextBoxStyle Normal, Meter, NoBackground
  - Added more values to the graphics table
  - bug fixes
</details>


# keywords currently incorporated:
## code blocks
tab through each entry for quicker coding. if a key has a choice of values, intellisense will show all optional values
### Controls
`ctrl` or `controls`<br>
Will build out the controls code block. more properties can be added once you tab through the base properties.
```
  table.insert(ctrls, {
    Name = "",
    Count = 1,
    ControlType = "Button | Indicator | Knob | Text"
  })
```
### Properties
`prop` or `properties`
will biuld out the table insersion for properties and add properties that are used the most.
```
table.insert(graphics, {
    Type = 
    Image = 
    Position = 
    Size = 
  })
```

### Graphics
`graphics`
will add to the controlLayouts table
```
table.insert(graphics, {
    Type = Label | GroupBox | Header | Image | SVG
    Image = 
    Position = 
    Size = 
  })
```

### Layout
`layout`
Will add the control to the Layout
```
layout["<control name>"] = {
  PrettyName = "<control name>",
  Style = "Button | Text | Fader | Knob | Meter | Led | ListBox | ComboBox | None",
  Position = {X, Y},
  Size = {X, Y}
  }
```

=======
## Getting Started
This extension is designed to be intuitive for users familiar with Q-SYS and VS Code. Simply type in the provided keywords to trigger IntelliSense and insert code blocks.

### Installation
Until I get it approved on the vscode market you will have to:
- download the .vsix file
- Open VScode
- navigate to the extentions tab
- click on the 3 dots above the search bar
- in the dropdown menu choose "install from vsix"

~~Install the extension directly from the Visual Studio Code Marketplace.~~

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
>>>>>>> 08fe7588c08c5a920a7c29c52ea5796e4941c9d0

### Graphics (`graphics`)
Adds entries to the `controlLayouts` table.

<<<<<<< HEAD
## Individual Keywords
- HTextAlign      - Left | Center | Right
- Position        - x | y
- Size            - x | y
- ButtonType      - Momentary | Toggle |Trigger | On | Off | Custom | StateTrigger
- IndicatorType   - Led | Meter | Text | Status
- UserPin         - true | false
- PinStyle        - Input | Output | Both | None
- Comment         - String (v9.10)
- Header          - String (v9.10)
- TextBoxStyle    - TextBoxStyle Normal | Meter | NoBackground
=======
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
>>>>>>> 08fe7588c08c5a920a7c29c52ea5796e4941c9d0
