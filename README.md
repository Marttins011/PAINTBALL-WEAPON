# PAINTBALL-WEAPON
Addon paintball weapon to use with mt-paintball to QBCore

# Installation:
Add to qb-core/shared/weapons.lua

```

[`weapon_paintball`]					= {['name'] = 'weapon_paintball',				['label'] = 'PaintBall Weapon',						['ammotype'] = nil,						['damagereason'] = 'Painted'},
  
```

Add to qb-core/shared/items.lua

```

	['weapon_paintball'] 			 = {['name'] = 'weapon_paintball', 		 	  	['label'] = 'PaintBall Weapon', 			    ['weight'] = 1000, 		['type'] = 'weapon', 	['ammotype'] = 'AMMO_PISTOL',			['image'] = 'weapon_paintball.png', 		['unique'] = true, 		['useable'] = false, 	['description'] = 'Paint your friends with this :)'},

```

Add to qb-smallresources/client/weapondraw.lua

```

	'WEAPON_PAINTBALL',
  
```

Add to qb-weapons/config.lua at Config.DurabilityMultiplier

```

    ['weapon_paintball'] 		= 0.0,

```

Add to qb-weapons/config.lau at Config.WeaponRepairCosts

```

    ['WEAPON_PAINTBALL'] = {
        ['defaultclip'] = {
            component = 'COMPONENT_PAINTBALL_CLIP_01',
            item = 'pistol50_defaultclip',
            type = 'clip',
        },
    },

```

Add to qb-ambulancejob/config.lua

```

    [`WEAPON_PAINTBALL`] = Config.WeaponClasses['NONE'],

```

Add to qb-smallresources/client/recoil.lua

```

[GetHashKey("weapon_paintball")] = 0.3,

```

Add this image to qb-inventory/html/images with name: weapon_paintball.png
![weapon_paintball](https://user-images.githubusercontent.com/89866234/176182369-577c6279-54fa-4693-a78e-a6b276cc8194.png)

# Weapon Model and skin credits:
https://pt.gta5-mods.com/weapons/paintball-gun
