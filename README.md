# fx-menu
RedM Menu System

# insatallation

- `ensure fx-menu` in the top of your resources.cfg 

# features
- Custom designe Fixitfy.
- Very easy to use.
- To use the icons you can use your png names in the file path "vorp_inventory/html/img/items" for vorpcore. For example icon = "cash"
- If you are using another framework, update the openmenu function in client/main.lua line 13 for the icons file path

# Credit
* credit goes to the QBCORE and RSGCore team for basecode and functionality
# Example
```lua
RegisterCommand('testmenu', function(args)
    exports['fx-menu']:openMenu({
        {
            header = "Rebels Menü",
            isMenuHeader = true,
        },
        {
            header = "Player's ID: 1",
            txt = "nixo dev",
            icon   = 'confirm',
            params = {
                event = "",
                isServer = false,
                args = {},
            }
        },
        {
            header = "Oyuncunun Mesleği",
            txt = "Cowboy",
            icon   = 'badge',
            params = {
                event = "",
                isServer = false,
                args = {},
            }
        },
        {
            header = "Oyuncunun Nakiti",
            txt = "100 $",
            icon   = 'money',
            params = {
                event = "",
                isServer = false,
                args = {},
            }
        },
        {
            header = "Oyuncunun Altını",
            txt = "0 Altın",
            icon = 'goldbar',
            params = {
                event = "",
                isServer = false,
                args = {},
            }
        },
        {
            header =  "Menüyü Kapat",
            txt = 'Çıkış',
            icon = "cancel",
            params = {
                event = 'fx-menu:closeMenu',
            }
        },
    })
end)
```
# Media
![fixit](https://github.com/Fixitfy/fx-menu/assets/139653962/bde42eec-b1d3-416b-93d5-d5ad5d9d6277)
![Screenshot_381](https://github.com/Fixitfy/fx-menu/assets/139653962/6927e1be-ae3a-4d05-8ace-c8f4dcae8a05)

