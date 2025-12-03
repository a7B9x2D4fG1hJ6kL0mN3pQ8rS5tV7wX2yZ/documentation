# Paramètre dans 'custom'

```lua
function maFonction(text)
    console.print(text, console.blue)
end
function move()
    return {
        { map = "-5,13", custom = (function() maFonction("Salut !") end) }
    }
end
```
