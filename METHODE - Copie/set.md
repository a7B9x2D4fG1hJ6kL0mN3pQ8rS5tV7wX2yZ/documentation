# set

{% hint style="success" %}
Méthode permettant de garder en mémoire du jeu une variable.
{% endhint %}

## 🔍 Prototype

```lua
memory.set(name, value)
```

## 📝 Paramètres

| Paramètre               | Type                                                                           | Description                                 |
| ----------------------- | ------------------------------------------------------------------------------ | ------------------------------------------- |
| <ul><li>name</li></ul>  | <ul><li>string</li></ul>                                                       | <ul><li>Le nom de la variable.</li></ul>    |
| <ul><li>value</li></ul> | <ul><li>string</li><li>bool</li><li>int</li><li>float</li><li>double</li></ul> | <ul><li>La valeur de la variable.</li></ul> |

## 🔙 Retour

| Type                           | Description                                                                      |
| ------------------------------ | -------------------------------------------------------------------------------- |
| <ul><li>false (bool)</li></ul> | <ul><li>Si le type du paramètre <code>value</code> n'est pas respecté.</li></ul> |
| <ul><li>true (bool)</li></ul>  | <ul><li>En cas de succès.</li></ul>                                              |
