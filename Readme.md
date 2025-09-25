# Library This UI Made by 96soul

Load
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/KUYKUBZ/Library/refs/heads/main/96soul.lua"))();
```
Create Windows
```lua
local Window = Library:New({
	logo = 137425711541503,
	bind = Enum.KeyCode.Q
})
-- _G.TabColor = ColorSequence.new{ColorSequenceKeypoint.new(0, Color3.fromRGB(255,0,0)),ColorSequenceKeypoint.new(0.5, Color3.fromRGB(255,140,0)),ColorSequenceKeypoint.new(1, Color3.fromRGB(255,140,0))}
```
Create tab
```lua
local Tab = Window:AddTab("General")
```
Create Section
``` lua
local left =  Tab:Section({
	title = "Section",
	side = "l" -- or r
})
```
Create Button
```lua
left:Button({
	title = "Button",
	callback = function()
		print("Click")
	end
})
```
Create Line
```lua
left:Line()
```
Create Toggle
```lua
left:Toggle({
	title = "Automatic",
	value = true,
	callback = function(v)
		print(v)
	end
})
```
Create Dropdown
```lua
left:Dropdown({
	Title = "Dropdown",
	Multi = false,
	List = {"Hello", "EZ"},
	Value = "Hello",
	Callback = function(v)
		print(v)
	end
})
```
Create Textbox
```lua
left:Textbox({
	Value = "Textbox",
	PlaceHolder = "Paste",
	ClearOnFocus = false,
	Callback = function(v)
		print(v)
	end
})
```
Create Slider
```lua
left:Slider({
	Title = "Slider",
	Value = 50,
	Min = 10,
	Max = 100,
	Rounding = 0,
	CallBack = function(v)
		print(v)
	end
})
```
Create Label
```lua
left:Label('This UI Made by <font color="rgb(0, 255, 127)">96soul</font>')
```

