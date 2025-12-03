# Faute à éviter en groupe

Supposons que vous voulez utiliser la <mark style="color:$primary;">potion de rappel</mark> sur la map <mark style="color:$primary;">164575663</mark>, certains vont faire ça :

```lua
function move()
    if map.onMap("164575663") then
        inventory.useObject(548)
    end
end
```

{% hint style="info" %}
Ici, seul le chef va utiliser la <mark style="color:$primary;">potion de rappel</mark>.
{% endhint %}

```lua
function popo()
    inventory.useObject(548)
end
function move()
    return {
        { map = "164575663", custom = popo },
    }
end
```

{% hint style="info" %}
Ici, toute la team va utiliser la <mark style="color:$primary;">potion de rappel</mark>.
{% endhint %}
