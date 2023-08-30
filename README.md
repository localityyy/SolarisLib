[![discord server](https://cdn.discordapp.com/attachments/832371927740973078/1146320361261117480/solaris2.png)](https://discord.gg/jaunk8nhN5)

# SolarisLib
Solaris Library is a free and open sourceed Roblox Ui Library
## SolarisLib script (don't use loadstring because it is bugged apparently!)
obviously you have to enter the link, if you only put the raw link it will not work for you at all
```lua
https://raw.githubusercontent.com/RegularRDev/SolarisLib/main/SolarisLib
```
## Important!
Solaris notifications don't work because your rbxassetdid is removed!

## Features:
- Customizable Options
- Browser-Like navigation
- Buttons
- Togles
- Sliders
- Dropdowns
- Keybinds
- Labels

## Documentation

### Get the Library
```lua
https://raw.githubusercontent.com/RegularRDev/SolarisLib/main/SolarisLib
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
### Create a sectiob
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
   your script or something
end)
```
### Sliders
```lua
local slider = sec:Slider("Slider", 0,25,0,2.5,"Slider", function(t)
   your script or something
end)
```
### Dropdowns
```lua
local dropdown = sec:Dropdown("Dropdown", {"a","b","c","d","e"},"","Dropdown", function(t)
   your scripts or something
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
### Keybinds
```lua
local label = sec:Label("Label")
```
