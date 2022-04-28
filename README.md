# BKHAX-UiLib
## Description
This Roblox ui library based on free and open source ui library. i forget original ui library name but yeah free to use everyone!

[How to use](#how-to-use)

[Component](#component)

[Example](#example)


## How to use
- Create a variabe name Library and loadstring from ```libs.lua```
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/NiZXD471/BKHAX-UiLib/main/libs.lua",true))()
```
- Then you can create new window by type
```lua
local win1 = Library:NewWindow("Any Name")
```
- After you create window then you need create a section by type
```lua
local sec1 = Library:NewSection("Any Name")
```
- And now after you create a section then you can put any component into the section
[All component](#component)


## Component
[Text Label](#text-label)

[Toggle](#toggle)

[Slider](#slider)

[Color Picker](#color-picker)

[Button](#button)

[Text Box](#text-box)

[Dropdown](#dropdown)

### Text Label
- You can create the text label by type **Require argument** (Name)
```lua
local label1 = sec1:CreateTextLabel("Hi mom")
```
- And you can update the text by type **Require argument** (Name)
```lua
label1:SetState("Hi dad")
```
You wanna go back to all comp? here >> [Back to Component](#component)



### Toggle
- You can create the toggle by type **Require argument** (Name,Function)
```lua 
local toggle1 = sec1:CreateToggle("What is this toggle!??",function(val)
    print(val)
    -- sum stuff here
end)
```
- And you can update the toggle by type **Require argument** (Boolean)
```lua
toggle1:SetState(true)
```
You wanna go back to all comp? here >> [Back to Component](#component)

### Slider
- You can create the slider by type **Require argument** (Name,Min,Max,StartValue,PreciseValue,Function)
```lua 
local slide1 = sec1:CreateSlider("AmSpeed",1,99,1,1,function(val)
    print(val)
    -- sum stuff here
end)
```
- And you can update the slider by type **Require argument** (Number)
this will set the value of a slider
```lua
slide1:SetState(true)
```
You wanna go back to all comp? here >> [Back to Component](#component)


### Color Picker
- You can create the color picker by type **Require argument** (Name,PresetColor,Function)
```lua 
local coolors = sec1:CreateColorPicker("Color picker?","I have no idea what is PresetColor i never use it before",function(val)
    print(val)
    -- sum stuff here
end)
```
You wanna go back to all comp? here >> [Back to Component](#component)


### Button
- You can create the button by type **Require argument** (Name,Function)
```lua 
local button1 = sec1:CreateButton("A button",function(val)
    print(val)
    -- sum stuff here
end)
```
- And you can update the button by type **Require argument** (Text)
```lua
button1:SetState("A button")
```
You wanna go back to all comp? here >> [Back to Component](#component)



### Text Box
- You can create the text box by type **Require argument** (Name,Function)
```lua 
local textbox1 = sec1:CreateTextbox("A text and box",function(val)
    print(val)
    -- sum stuff here
end)
```
- And you can update the text box by type **Require argument** (Text)
```lua
textbox1:SetState("A text and box update!")
```
You wanna go back to all comp? here >> [Back to Component](#component)



### Dropdown
- You can create the dropdown by type **Require argument** (Name,Table,Presetoption,Function)
```lua 
local dropdown1 = sec1:CreateDropdown("Select food",{"Hamberger","Hot dog","Pine apple"},1,function(val)
    print(val)
    -- sum stuff here
end)
```
- You can update the dropdown by type **Require argument** (Value)
```lua
dropdown1:SetState("A text and box update!")
```

- You can clear the dropdown by type
```lua
dropdown1:Clear()
```

- And you can refresh the dropdown by type **Require argument** (Table)
```lua
dropdown1:Clear()
```
You wanna go back to all comp? here >> [Back to Component](#component)









## Example
These are the example of how to use ui libs
- Slide da speed
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/NiZXD471/BKHAX-UiLib/main/libs.lua",true))()

local win1 = Library:NewWindow("BKHAX")
local sec1 = win1:NewSection("Speed")
local slide1 = sec1:CreateSlider("Set speed",1,100,50,10,function(val)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = val
end)
```

![Image](https://raw.githubusercontent.com/NiZXD471/BKHAX-UiLib/main/Image/Slide%20da%20speed.png)
