# BlekLib

BlekLib is a open sourced Roblox UI library inspired by Dark Hub
Support server: discord.gg/zen

## Loadstring
```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/laderite/bleklib/main/library.lua"))()
```

## Features:
- Buttons
- Sliders
- Textbox
- Toggles
- Labels

- dropdowns soon

## Documentation
Shows an example of all the ui elements

# Load the library
```lua
local BlekLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/laderite/bleklib/main/library.lua"))()
```

# Creating the UI
```lua
local win = BlekLib:Create({
    Name = "Blek Library",
    StartupSound = {
        Toggle = false,
        SoundID = "rbxassetid://6958727243",
        TimePosition = 1
    }
})
```

# Creating a tab
```lua
local maintab = win:Tab('Main')
local charactertab = win:Tab('Character')
local uitab = win:Tab('UI')
```

# Creating a button
```lua
uitab:Button('Destroy GUI', function()
    win:Exit()
end)
```

# Creating a toggle
```lua
maintab:Toggle('Aimbot', function(v)
    aimbot = v
end)
```

# Creating a textbox
```lua
maintab:Textbox('FOV', function(v)
    fov = v
end)
```

# Creating a slider
```lua
maintab:Slider('FOV', 30 -- default, 10 -- min, 300 -- max, function(a)
    print(a)
end)
```

# Creating a label
```lua
maintab:Label('This is a label')
```
