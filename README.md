# Q-SYS VSCode Extension

## Overview
qsys-vscode-extension is an extension for Visual Studio Code designed specifically for Q-SYS plugin development. It provides IntelliSense support and a set of snippets tailored for the Q-SYS Basic Plugin Framework, streamlining the plugin creation process.

## Features
- **IntelliSense Integration**: Enhances coding efficiency with Q-SYS plugin development by offering IntelliSense support.
- **Code Snippets**: A collection of snippets that can be inserted using keywords, speeding up the coding process.

## Getting Started
This extension is designed to be intuitive for users familiar with Q-SYS and VS Code. Simply type in the provided keywords to trigger IntelliSense and insert code blocks.

### Installation
Install the extension directly from the Visual Studio Code Marketplace.

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
    ControlType = "Button | Indicator | Knob | Text",
    UserPIn = true | false,
    PinStyle = "Input | Output | Both | None"
  })
```

### Properties
`prop` or `properties`
will biuld out the table insersion for properties and add properties that are used the most.
```
table.insert( props, {
      Name = "Count",
      Type = "integer",
      Value = 8,
      Min = 2,
      Max = 64,
      Comment = "Range: 2-64",
      Header = "Channels"
    }
  )
```

### Component
`components`
Will populate the basic must haves for component creation
```
table.insert(components, {
  Name = "",
  Type = "",
  Properties = {}
})
```

### Graphics
`graphics`
will add to the controlLayouts table
``` 
table.insert(graphics, {
    Type = Label | GroupBox | Header | Image | SVG
    Image = "",
    Position = {,},
    Size = {,},
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

### GroupBox
`GroupBox`
Will populate the GroupBox table
```
table.insert(graphics, {
  Type = GroupBox,
  Text = "",
  HTextAlign = "Center | Left | Right",
  Size = {x,y},
  Position = {x,y},
  CornerRadius = integer
})
```

## Individual Keywords
- HTextAlign      - Left | Center | Right
- Position        - x | y
- Size            - x | y
- ButtonType      - Momentary | Toggle |Trigger | On | Off | Custom | StateTrigger
- ButtonStyle     - Toggle | Momentary | Trigger | On | Off | Custom
- ButtonVisualStyle - Flat | Gloss
- IndicatorType   - Led | Meter | Text | Status
- UserPin         - true | false
- PinStyle        - Input | Output | Both | None
- MeterStyle      - Level | Reduction | Gain | Standard
- ControlUnit     - dB | Hz | Float | Integer | Pan | Percent | Position | Seconds
- Comment         - String (v9.10)
- Header          - String (v9.10)
- TextBoxStyle    - Normal | Meter | NoBackground

## Version History
<details>
 <summary><b>Version 1.1.0</b></summary>

  - Added Comment and Header for optional strings on properties
  - Added ButtonType  On, Off , Custom, StateTrigger
  - Added TextBoxStyle Normal, Meter, NoBackground
  - Added more values to the graphics table
  - bug fixes
</details>

<details>
 <summary><b>Version 1.2.0</b></summary>

 - Lots of bug fixes
 - Adding more options for properties that came out with 9.10
 - Adding more keywords
</details>

<details>
 <summary><b>Version 1.2.3</b></summary>

   - fixing x, y placeholders on position and size values
</details>

<details>
 <summary><b>Version 1.2.4</b></summary>

   - ControlUnit: Removing $ within the curly brackets. Fixes issue with snippet not populating correctly.
</details>

<details>
 <summary><b>Version 1.2.5</b></summary>

   - Removing tab indent for Layout
   - Fixing formatting for ButtonStyle
</details>

## Contributing
This project is open to public contributions. Feel free to add new features, improve existing ones, or suggest changes. Your input is valuable in making this tool more effective for everyone.

## License
This extension is released under an open-source license, inviting widespread collaboration and modification.

## Notes
- Ensure you are familiar with the Q-SYS Basic Plugin Framework for effective use of this extension.
- This extension is in active development; stay tuned for more updates and features.

