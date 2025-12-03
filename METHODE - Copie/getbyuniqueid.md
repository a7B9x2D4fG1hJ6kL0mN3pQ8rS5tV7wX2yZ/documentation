# getByUniqueId

{% hint style="success" %}
Méthode permettant de récupérer l'identifiant d'une fenêtre du jeu, à utiliser sur pour méthodes de [ipc](https://doc.frigost.dev/abonnement-frigost-bot/methodes/ipc), [mouse](https://doc.frigost.dev/abonnement-frigost-bot/methodes/mouse), [keyboard](https://doc.frigost.dev/abonnement-frigost-bot/methodes/keyboard) et [pixel](https://doc.frigost.dev/abonnement-frigost-bot/methodes/pixel).
{% endhint %}

## 🔍 Prototype

```lua
window.getByUniqueId(uniqueId)
```

## 📝 Paramètres

| Paramètre                  | Type                  | Description                                                                                                                                                                                                                                                                                      |
| -------------------------- | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <ul><li>uniqueId</li></ul> | <ul><li>int</li></ul> | <ul><li>Identifiant unique à paramétrer ici :<br><img src="https://3373271050-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-Mfulp0LhbJrdkH_fl5w%2Fuploads%2FNQ57XFNugA71wL8nfubt%2Fimage.png?alt=media&#x26;token=b3954dee-1447-4698-98fb-04a0f62818b5" alt=""></li></ul> |

## 🔙 Retour

| Type                   | Description                                           |
| ---------------------- | ----------------------------------------------------- |
| <ul><li>HWND</li></ul> | <ul><li>L'identifiant de la fenêtre du jeu.</li></ul> |
| <ul><li>nil</li></ul>  | <ul><li>Si introuvable.</li></ul>                     |
