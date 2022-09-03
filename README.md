# Starterkit Skript

command /starter:
    permission: starterkit.use
    trigger:
        if {starter.items.%uuid of player%} is not set:
            give 1 stone sword to player
            give 1 stone axe to player
            give 1 stone pickaxe to player
            give 1 stone shovel to player            
            give 16 steak to player
            equip player with chain leggings
            equip player with chain chestplate
            
            set {starter.items.%uuid of player%} to true
            send "§l§cStarterItems§l§c §e>>>§e §a§Sie haben die Starter-Items erhalten!§o§a"   
        else:
            send "§l§cStarterItems§l§c §e>>>§e §c§oSie haben Ihre Starter-Items bereits erhalten!§o§c"

command /starterhelp:
    permission: starterkit.help
    trigger:
        send "§f==========================================================================§f"
        send ""
        send "§l§c                        §c§lStarterItems§c §f- Commands§l:§f"
        send ""
        send "§l§a/starter§a§l §f- §oGibt dir Die Starter Items§o§f"
        send "§l§a/delstarter§a§l §f- §oSetzt deine Starter-Items zurück, damit du sie wieder bekommen kannst (Admin Command)"
        send "§l§a/starterhelp§a§l §f- §oZeigt dir diese Liste an"
        send ""
        send "§l§aProject by FloCrafterHD"
        send "§f==========================================================================§f"
        
# by FloCrafterHD
#Skript-Coding
# Wichtig Bitte die datei starter.sk downloaden und nicht die readme.md

# Permissions
starterkit.use
starterkit.help

