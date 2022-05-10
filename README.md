Sl Sweet House For your server

# Dependencies
* [qbcore framework](https://github.com/qbcore-framework)
* [qb-target](https://github.com/BerkieBb/qb-target)
* [qb-core](https://github.com/qbcore-framework/qb-core)
* [qb-shops](https://github.com/qbcore-framework/qb-shops)
* [qb-smallresources](https://github.com/qbcore-framework/qb-smallresources)

## Insert images @qb-inventry --> html --> images
```
In the Images Folder
```

## Insert into @qb-smallresources --> server --> consumables.lua
```

--sl sweet

QBCore.Functions.CreateUseableItem("marie", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("lion_bun", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("chocos", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("minichips", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("chocolate_biscuit", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("rovello_chocolate", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("stix_vanillae", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("stix_chocolat", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("stix_straberry", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)
```

## Insert into @qb-smallresources --> config.lua
```
ConsumeablesEat = {

    --slsweet

    ["lion_bun"] = math.random(35, 54),
    ["chocos"] = math.random(35, 54),
    ["minichips"] = math.random(35, 54),
    ["chocolate_biscuit"] = math.random(35, 54),
    ["rovello_chocolate"] = math.random(35, 54),
    ["stix_vanilla"] = math.random(35, 54),
    ["marie"] = math.random(35, 54),
    ["stix_chocolate"] = math.random(35, 54),
    ["stix_straberry"] = math.random(35, 54),
     }
```

## Insert into @qb-core/shared/items.lua
```

--sl foods eat itmes
	['lion_bun'] 				= {['name'] = 'lion_bun', 			  	 ['label'] = 'Lion_Bun', 			['weight'] = 200, 	['type'] = 'item', 	['image'] = 'lion_bun.png', 				['unique'] = false, ['useable'] = true, 	['shouldClose'] = true,	   	['combinable'] = nil,   ['description'] = 'Sri Lanka Buns for your stomach'},
	['chocos'] 					= {['name'] = 'chocos', 			  	 ['label'] = 'Chocos', 				['weight'] = 200, 	['type'] = 'item', 	['image'] = 'chocos.png', 					['unique'] = false, ['useable'] = true, 	['shouldClose'] = true,	   	['combinable'] = nil,   ['description'] = 'Sri Lanka Chocos for your stomach'},
	['minichips'] 				= {['name'] = 'minichips', 			  	 ['label'] = 'Minichips', 			['weight'] = 200, 	['type'] = 'item', 	['image'] = 'minichips.png', 				['unique'] = false, ['useable'] = true, 	['shouldClose'] = true,	   	['combinable'] = nil,   ['description'] = 'Sri Lanka minichips for your stomach'},
	['chocolate_biscuit'] 		= {['name'] = 'chocolate_biscuit', 		 ['label'] = 'chocolate Biscuit', 	['weight'] = 200, 	['type'] = 'item', 	['image'] = 'chocolate_bis.png', 			['unique'] = false, ['useable'] = true, 	['shouldClose'] = true,	   	['combinable'] = nil,   ['description'] = 'Sri Lanka chocolate biscuit for your stomach'},
	['rovello_chocolate'] 		= {['name'] = 'rovello_chocolate', 		 ['label'] = 'Rovello Chocolate', 	['weight'] = 200, 	['type'] = 'item', 	['image'] = 'rovello_chocolate.png', 		['unique'] = false, ['useable'] = true, 	['shouldClose'] = true,	   	['combinable'] = nil,   ['description'] = 'Sri Lanka rovello chocolate for your stomach'},
	['marie'] 					= {['name'] = 'marie', 		 			 ['label'] = 'Gold Marie', 			['weight'] = 200, 	['type'] = 'item', 	['image'] = 'marie.png', 					['unique'] = false, ['useable'] = true, 	['shouldClose'] = true,	   	['combinable'] = nil,   ['description'] = 'Sri Lanka Gold Marie for your stomach'},
	['stix_vanilla'] 			= {['name'] = 'stix_vanilla', 		 	 ['label'] = 'Stix Vanilla', 		['weight'] = 200, 	['type'] = 'item', 	['image'] = 'stix_vanilla.png', 			['unique'] = false, ['useable'] = true, 	['shouldClose'] = true,	   	['combinable'] = nil,   ['description'] = 'Sri Lanka Stix Vanilla for your stomach'},
	['stix_chocolate'] 			= {['name'] = 'stix_chocolate', 		 ['label'] = 'Stix Chocolate', 		['weight'] = 200, 	['type'] = 'item', 	['image'] = 'stix_chocolate.png', 			['unique'] = false, ['useable'] = true, 	['shouldClose'] = true,	   	['combinable'] = nil,   ['description'] = 'Sri Lanka Stix Chocolate for your stomach'},
	['stix_straberry'] 			= {['name'] = 'stix_straberry', 		 ['label'] = 'Stix Straberry', 		['weight'] = 200, 	['type'] = 'item', 	['image'] = 'stix_straberry.png', 			['unique'] = false, ['useable'] = true, 	['shouldClose'] = true,	   	['combinable'] = nil,   ['description'] = 'Sri Lanka Stix Straberry for your stomach'},
```
## Insert into @qb-smallresources --> config.lua
```
Config.Products = {
    --sl shop
    ["slsweet"] = {
        [1] = {
            name = "lion_bun",
            price = 5,
            amount = 50,
            info = {},
            type = "item",
            slot = 1,
        },
        [2] = {
            name = "chocos",
            price = 4,
            amount = 50,
            info = {},
            type = "item",
            slot = 2,
        },
        [3] = {
            name = "minichips",
            price = 4,
            amount = 50,
            info = {},
            type = "item",
            slot = 3,
        },
        [3] = {
            name = "rovello_chocolate",
            price = 8,
            amount = 50,
            info = {},
            type = "item",
            slot = 3,
        },
        [4] = {
            name = "chocolate_biscuit",
            price = 6,
            amount = 50,
            info = {},
            type = "item",
            slot = 4,
        },
        [5] = {
            name = "marie",
            price = 6,
            amount = 50,
            info = {},
            type = "item",
            slot = 5,
        },
        [6] = {
            name = "marie",
            price = 6,
            amount = 50,
            info = {},
            type = "item",
            slot = 6,
        },
        [7] = {
            name = "stix_vanilla",
            price = 3,
            amount = 50,
            info = {},
            type = "item",
            slot = 7,
        },
        [8] = {
            name = "stix_chocolate",
            price = 3,
            amount = 50,
            info = {},
            type = "item",
            slot = 8,
        },
        [9] = {
            name = "stix_straberry",
            price = 3,
            amount = 50,
            info = {},
            type = "item",
            slot = 9,
        },
    },
}
    Config.Locations = {
    --slsweet
    ["slsweet"] = {
        ["label"] = "SL Sweet House",
        ["coords"] = vector4(272.53, -965.04, 29.31, 37.29),
        ["ped"] = 'mp_m_shopkeep_01',
        ["scenario"] = "WORLD_HUMAN_STAND_MOBILE",
        ["radius"] = 1.5,
        ["targetIcon"] = "fas fa-shopping-basket",
        ["targetLabel"] = "Open Shop",
        ["products"] = Config.Products["slsweet"],
        ["showblip"] = true,
        ["blipsprite"] = 52,
        ["blipcolor"] = 1
    },
    }
```
