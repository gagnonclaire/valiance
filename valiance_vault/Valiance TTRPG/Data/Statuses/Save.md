---
{
	"name": "save",
	"tags": [ "global", "ability" ],
	"tier": 0,
	"target": character,
	"energy-cost": 1,
	"properties": [
		{
			"name": "action",
			"value": 1, 
		},
		{
			"name": "range",
			"value": 1,
			"secondary_value": 1, # not technically needed, if we have no secondary we just assume it's the same as primary (for range property)
		},
	],	
	"effect": "Clear one point of any ailment affecting the target",
	"flavor-text": "Valiants rarely work alone, and for good reason.",
}
---
In code, we have "ability" objects that hold functions based on name. For example, we have a "save" object that inherits the "ability" prototype object and implements its "on_use" function. The "on_use" function would probably take a "user" and "target" parameter along with an "options" and then do its thing. In this case, it would check usage validity based on the user and target, then look at the options param to determine which ailment to reduce.

Have error handling (vs hard crash) for:
- no user (every ability needs a user)
- no target (some abilities are exempt, such as strategies that affect the whole field)
- required options not found

May be some better way to store this game data, or even to generate it? Want to keep the ability to have all necessary pieces readable externally so we can gen rule docs with it.

