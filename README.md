# qsys-vscode-extension
extension for VS Code that incorporates intellisense for qsys plugin creation.

meant to be used with the q-sys basic plugin framework

some snippets can be inserted by keywords. 

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


### layout
will add to the layout table and add properties that are use the most.

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
