# Boris Ui
#### very nice and small and sexy all da ladies luv it ;)


### Setup The Library

```lua
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/pzfp5vpksc-droid/deuiobdoom/refs/heads/main/uistuff", true))()
```

### Adding Window

```lua
local Window = library:CreateWindow("Your Title")
```
### Adding Tab Inside Of Window (Optional)

```lua
local Tab = tab:AddFolder("Tab1")
```
### Adding Button

```lua
Window:AddButton({
	text = "Click Me",
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
	min = 10,
	max = 100,
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
    text = "Fruit",
    values = {"Apple", "Banana", "Pear"},
    callback = function(value)
        print("Selected fruit:", value)
    end,
    open = false,
    flag = "fruits"
})
```

### Adding A Bind

```lua
Window:AddBind({
    text = "Bind",
    key = "C",
    hold = false,
    callback = function()
    end
})
```

### Adding A Label

```lua
Window:AddLabel({
	text = "You Have Aura.",
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
