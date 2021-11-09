# QB-ARCADE
Arcade script for Qb


# Required
***[qb-target](https://github.com/BerkieBb/berkie-target)***

***[casinoUi](https://github.com/dojwun/casinoUi)***

***[qb-menu](https://github.com/qbcore-framework/qb-menu)***

***[ms-peds-dev] (https://forum.cfx.re/t/release-ped-spawner/2462689)***

***[patoche cyber bar] (https://forum.cfx.re/t/mlo-cyber-bar-v2/4769478)***



***add this to ms-peds-dev***
	
--arcade ped 
	{
		model = `cs_lifeinvad_01`, -- Model name as a hash.
		coords = vector4(334.63, -907.82, 29.26, 70.05),
		gender = 'male' -- The gender of the ped, used for the CreatePed native.
	},




# Images 

![General](https://i.imgur.com/5bLve6O.png)
![General](https://i.imgur.com/815vDIQ.png)
![General](https://i.imgur.com/czXFSze.png)


- qb-core/shared.lua info
```
	["arcadegreen"]  = {
		["name"] = "arcadegreen",
		["label"] = "Green Arcade Card",
		["weight"] = 0, 		
		["type"] = "item", 		
		["image"] = "arcadegreen.png", 		
		["unique"] = true, 		
		["useable"] = false, 	
		["shouldClose"] = false,	   
		["combinable"] = nil,   
		["description"] = "Green Arcade Card"
	},
	["arcadeblue"]  = {
		["name"] = "arcadeblue",
		["label"] = "Blue Arcade Card",
		["weight"] = 0, 		
		["type"] = "item", 		
		["image"] = "arcadeblue.png", 		
		["unique"] = true, 		
		["useable"] = false, 	
		["shouldClose"] = false,	   
		["combinable"] = nil,   
		["description"] = "Blue Arcade Card"
	},
	["arcadegold"]  = {
		["name"] = "arcadegold",
		["label"] = "Gold Arcade Card",
		["weight"] = 0, 		
		["type"] = "item", 		
		["image"] = "arcadegold.png", 		
		["unique"] = true, 		
		["useable"] = false, 	
		["shouldClose"] = false,	   
		["combinable"] = nil,   
		["description"] = "Gold Arcade Card"
	},
 ``` 
- qb-inventory/html/js/app.js
```
	  else if (itemData.name == "arcadeblue") {
            $(".item-info-title").html('<p>'+itemData.label+'</p>')
            $(".item-info-description").html('<p><strong>Owner: </strong>'+itemData.info.owner+'</p><strong>Play Card Time:</strong> '+itemData.info.cardtime+' minutes</p>'); 
            $(".item-info-stats").html('<p>Weight: '+((itemData.weight * itemData.amount) / 1000).toFixed(1) +' | Amount: '+itemData.amount+ ' | Quality: '+itemData.info.quality.toFixed(0)+'%</p>') 
        } else if (itemData.name == "arcadegreen") {
            $(".item-info-title").html('<p>'+itemData.label+'</p>')
            $(".item-info-description").html('<p><strong>Owner: </strong>'+itemData.info.owner+'</p><strong>Play Card Time:</strong> '+itemData.info.cardtime+' minutes</p>'); 
            $(".item-info-stats").html('<p>Weight: '+((itemData.weight * itemData.amount) / 1000).toFixed(1) +' | Amount: '+itemData.amount+ ' | Quality: '+itemData.info.quality.toFixed(0)+'%</p>') 
        } else if (itemData.name == "arcadegold") {
            $(".item-info-title").html('<p>'+itemData.label+'</p>')
            $(".item-info-description").html('<p><strong>Owner: </strong>'+itemData.info.owner+'</p><strong>Play Card Time:</strong> '+itemData.info.cardtime+' minutes</p>'); 
            $(".item-info-stats").html('<p>Weight: '+((itemData.weight * itemData.amount) / 1000).toFixed(1) +' | Amount: '+itemData.amount+ ' | Quality: '+itemData.info.quality.toFixed(0)+'%</p>') 
        }
  ```
