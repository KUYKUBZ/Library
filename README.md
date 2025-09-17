# Library
Load
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/KUYKUBZ/Library/refs/heads/main/dearquiz.lua"))();
```
Create Windows
```lua
local Window = Library:New({
	logo = 84028960215079,
	bind = Enum.KeyCode.Q
})
```
Create tab
```lua
local Tab = Window:AddTab("General")
```
Create Section
``` lua
local left =  Tab:Section({
	title = "Section",
	side = "l"
})
```

local right =  Tab2:Section({
	title = "Section",
	side = "r"
})

left:Button({
	title = "Button",
	callback = function()
		print("Click")
	end
})

left:Line()

left:Toggle({
	title = "Automatic",
	value = true,
	callback = function(v)
		print(v)
	end
})

left:Toggle({
	title = "Automatic",
	value = false,
	callback = function(v)
		print(v)
	end
})

left:Dropdown({
	Title = "Dropdown",
	Multi = false,
	List = {"Hello", "EZ"},
	Value = "Hello",
	Callback = function(v)
		print(v)
	end
})

left:Dropdown({
	Title = "Dropdown Multi",
	Multi = true,
	List = {"Hello", "EZ"},
	Value = {"Hello"},
	Callback = function(v)
		print(v)
		--Dropdown:AddList("Hello") -- เพิ่มรายชื่อ
		--Dropdown:Clear("Hello") -- ลบรายชื่อแบบเลือก
		--Dropdown:Clear() -- ลบรายชื่อทั้งหมด
	end
})

right:Textbox({
	Value = "Textbox",
	PlaceHolder = "Paste",
	ClearOnFocus = false,
	Callback = function(v)
		print(v)
	end
})

right:Line()

right:Slider({
	Title = "Slider",
	Value = 50,
	Min = 10,
	Max = 100,
	Rounding = 0,
	CallBack = function(v)
		print(v)
	end
})

right:Line()

left:Line()

left:Label('This UI Made by <font color="rgb(0, 255, 127)">96soul</font>')


left:Line()

