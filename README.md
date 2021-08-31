# pvp-FiveM
Ce script active le pvp sur votre serveur GTA 5 RP FiveM
Vous pouvez aussi active le pvp en insérer ce bout de code coté client du essentialmode :

AddEventHandler("playerSpawned", function()
    NetworkSetFriendlyFireOption(true)
    SetCanAttackFriendly(PlayerPedId(), true, true)
end)

2 ème façon :
Dirigez vous dans essentialmode, puis dans client et enfin dans main.lua (ligne 58) et mettez ceci en true si ce n’est pas déjà fait :

RegisterNetEvent("es:enablePvp")
AddEventHandler("es:enablePvp", function()
    pvpEnable = true
end)

Et voilà, j’espère que vous avez réussi à résoudre votre problème.
