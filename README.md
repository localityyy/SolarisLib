# SolarisLib
Solaris Library is a free and open sourced Roblox Ui Library
## SolarisLib script (don't use loadstring because it is bugged apparently!) obviously you have to enter the link, if you only put the raw link it will not work for you at all
```lua
https://raw.githubusercontent.com/localityyy/SolarisLib/refs/heads/main/SolarisLib
```
## Important!
Solaris notifications don't work because the rbxassetdid is removed! 
Also, you can only put 11 sections as solaris can't scroll sections like other scripts

## Features:
- Customizable Options
- Browser-Like navigation (broken apparently lol)
- Buttons
- Toggles
- Sliders
- Dropdowns
- Colorpickers
- Textboxes
- Keybinds
- Labels

## Documentation

### Get the Library
```lua
https://raw.githubusercontent.com/localityyy/SolarisLib/refs/heads/main/SolarisLib
```

### Create the GUI
```lua
local win = SolarisLib:New({
    Name = "SolarisLib",
    FolderToSave = "SolarisLibStuff"
})
```

### Tabs
```lua
local tab = win:Tab("Example")
```
### Create a section
```lua
local sec = tab:Section("Section Example")
```
### Buttons
```lua
sec:Button("example", function()
    loadstring(game:HttpGet('an script'))()
end)
```
### Toggles
```lua
local toggle = sec:Toggle("Toggle", false,"Toggle", function(t)
    --your script or something
end)
```
### Sliders
```lua
local slider = sec:Slider("Slider", 0,25,0,2.5,"Slider", function(t)
    --your script or something
end)
```
### Dropdowns
```lua
--- Normal dropdowns
local dropdown = sec:Dropdown("Dropdown", {"a","b","c","d","e"},"","Dropdown", function(t)
    --your script or something
end)

--- multidropdowns
local multidropdown =sec:MultiDropdown("Multi Dropdown", {"a","b","c","d","e"},{"b", "c"},"Dropdown", function(t)
    print(table.concat(t, ", "))
end)
```
### Colorpickers
```lua
sec:Colorpicker("Colorpicker", Color3.fromRGB(255,255,255),"Colorpicker", function(t)
    print(t)
end)
```
### Textboxes
```lua
sec:Textbox("Textbox", true, function(t)
    print(t)
end)
```
### Keybinds
```lua
--- Hold bind
sec:Bind("Hold Bind", Enum.KeyCode.E, true, "BindHold", function(t)
    print(t)
end)

--- Normal Bind
sec:Bind("Normal Bind", Enum.KeyCode.F, false, "BindNormal", function()
    print("Bind pressed")
end)
```
### Labels
```lua
local label = sec:Label("Label")
```
### Script source Preview
```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/localityyy/SolarisLib/refs/heads/main/Preview"))()
```
Credits to Solaris team for the Library,
