---
{
	"name": "lead-core",
	"tags": [ "equipment", "weapon", "ability" ],
	"tier": 2,
	"base-item": "heavy-melee-weapon",
	"target": "character",
	"energy-cost": 1,
	"properties": [
		"action 2",
		"attack 0",
		"range 1",
	],
	"effect": "Deal piercing damage equal to three times the target character’s Resistance.",
	"check-effects": [
	{
		"result": "good",
		"effect": "Instead deal piercing damage equal to four times the target character’s Resistance."
	},
	{
		"result": "great",
		"effect": "Instead deal piercing damage equal to five times the target character’s Resistance."
	},
	{
		"result": "perfect",
		"effect": "Instead deal piercing damage equal to six times the target character’s Resistance."
	},
],
	"flavor-text": "Heavy metal poisoning is going to be the least of your concerns.",
}
---
