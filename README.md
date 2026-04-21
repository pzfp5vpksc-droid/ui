# Boris Ui
#### very nice and small and sexy all da ladies luv it :)


### Setup The Library

```lua
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/pzfp5vpksc-droid/deuiobdoom/refs/heads/main/uistuff", true))()
```

### Adding Tab

```lua
local Window = library:CreateWindow("Your Title")
```
### Adding Folder Inside Of Tab (Optional)

```lua
local folder = tab:AddFolder("Folder")
```
### Adding Button

```lua
Window:AddButton({
	text = "Click me",
	flag = "button",
	callback = function()
	print("hello world")
end
})
```
### Adding Toggle

```lua
Window:AddToggle({
	text = "Toggle",
	flag = "toggle",
	callback = function(v)
	print(v)
end
})
```
### Adding TextBox

```lua
Window:AddTextbox({
	text = "TextBox",
	flag = "textbox",
	callback = function(v)
	print(v)
end
})
```
### Adding A Slidder

```lua
Window:AddSlider({
	text = "Fov",
	min = 70,
	max = 170,
	dual = true,
	type = "slider",
	callback = function(v)
	print(v)
end
})
```

### Adding A DropDown

```lua
Window:AddList({
    text = "Color",
    values = {"Red", "Green", "Blue"},
    callback = function(value)
        print("Selected color:", value)
    end,
    open = false,
    flag = "color_option"
})
```

### Adding A Bind

```lua
Window:AddBind({
    text = "bind",
    key = "X",
    hold = false,
    callback = function()
    end
})
```

### Adding A Label

```lua
Window:AddLabel({
	text = "This Is Sick!",
	type = "label"
	})
```

### Close Library

```lua
library:Close()
```

### Final (REQUIRED OR THE UI WILL NOT SHOW)

```lua
library:Init()
```
