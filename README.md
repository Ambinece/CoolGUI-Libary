Basic repesentation of a script using this library:

```luau
local CoolGUI = loadstring(game:HttpGet("https://raw.githubusercontent.com/Ambinece/CoolGUI-Libary/refs/heads/main/CoolGUI"))()

-- Create the main window
local window = CoolGUI:CreateWindow({
    Title = "C00lGui"
})

-- Create a button
window:AddButton({
    Text = "Button",
    Callback = function()
        print("Hello world")
    end
})

-- Create a toggle
window:AddToggle({
    Text = "Toggle",
    Callback = function(state)
        if state then
            print("Enabled")
        else
            print("Disabled")
        end
    end
})

-- Change theme
CoolGUI:SetTheme("RedAndBlack") -- Only works if the theme exists
```
