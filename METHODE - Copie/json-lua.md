# JSON ⇆ LUA

Si vous voulez intégrer la lecture et écriture JSON dans vos scripts, mettez ce fichier à coté de votre script dans le meme dossier (à ne pas toucher ou modifier).

{% file src="<https://3373271050-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-Mfulp0LhbJrdkH_fl5w%2Fuploads%2FDxAe6hIGRE3QBDpRQK2e%2FJSON.lua?alt=media&token=d3e56340-24e5-47f7-bb40-3d94d5845155>" %}

Voici un exemple d'utilisation :&#x20;

```lua
-- Charger le module
JSONFile = script.folder().."\\JSON.lua"
JSON = (loadfile(JSONFile))()

function move()
    -- JSON vers LUA
    local mapDataString = map.data()
    local mapData = JSON:decode(mapDataString)
    console.print(mapData.x)
    
    -- LUA vers JSON
    local myTable = { 1, 2, { "a", "b" } }
    local myTableString = JSON:encode(myTable)
    console.print(myTableString)
end
```
