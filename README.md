# qsys-vscode-extension
extension for VS Code that incorporates intellisense for qsys plugin creation.

meant to be used with the q-sys basic plugin framework

some snippets can be inserted by keywords. 

<details>
 <summary><b>Version 1.0.1</b></summary>
  - bug fixes mainly.
</details>

# V 0.0.1
just begining stages. this is open to the public if anyone wants to add or modify anything. 
## keywords currently incorporated:
## code blocks
tab through each entry for quicker coding. if a key has a choice of values, intellisense will show all optional values
### ctrl or controls<br>
Will build out the controls code block. more properties can be added once you tab through the base properties.
```
  table.insert(ctrls, {
    Name = "",
    Count = 1,
    ControlType = "Button | Indicator | Knob | Text"
  }
```
### props or properties
will biuld out the table insersion for properties and add properties that are used the most.

### graphics
will add to the controlLayouts table

### layout
will add to the layout table and add properties that are use the most.

## Individual Keywords
### HTextAlign
### Position
### Size
### ButtonType
### IndicatorType
### UserPin
### PinStyle
