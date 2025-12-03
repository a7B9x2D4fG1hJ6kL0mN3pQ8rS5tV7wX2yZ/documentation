# getByTeamData

{% hint style="success" %}
Méthode permettant de récupérer l'identifiant d'une fenêtre du jeu, à utiliser sur pour méthodes de [ipc](https://doc.frigost.dev/abonnement-frigost-bot/methodes/ipc), [mouse](https://doc.frigost.dev/abonnement-frigost-bot/methodes/mouse), [keyboard](https://doc.frigost.dev/abonnement-frigost-bot/methodes/keyboard) et [pixel](https://doc.frigost.dev/abonnement-frigost-bot/methodes/pixel).
{% endhint %}

## 🔍 Prototype

```lua
window.getByTeamData(teamNumber, inTeamIndex)
```

## 📝 Paramètres

| Paramètre                     | Type                  | Description                                                    |
| ----------------------------- | --------------------- | -------------------------------------------------------------- |
| <ul><li>teamNumber</li></ul>  | <ul><li>int</li></ul> | <ul><li>Numéro de la team.</li></ul>                           |
| <ul><li>inTeamIndex</li></ul> | <ul><li>int</li></ul> | <ul><li>L'index (l'ordre) du compte dans cette team.</li></ul> |

## 🔙 Retour

| Type                   | Description                                           |
| ---------------------- | ----------------------------------------------------- |
| <ul><li>HWND</li></ul> | <ul><li>L'identifiant de la fenêtre du jeu.</li></ul> |
| <ul><li>nil</li></ul>  | <ul><li>Si introuvable.</li></ul>                     |
