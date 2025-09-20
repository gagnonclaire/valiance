---
{
	"name": "heavy-melee-weapon",
	"tags": [ "equipment", "weapon", "ability" ],
	"tier": 0,
	"target": character,
	"energy-cost": 0,
	"properties": [
		"action 2",
		"attack 1",
		"check",
		"range 1",
	],
	"effect": "Deal 6 damage.",
	"check-effects": [
		{
			"result": "good",
			"effect": "Deal 2 additional damage."
		},
		{
			"result": "great",
			"effect": "Deal 4 additional damage."
		},
		{
			"result": "perfect",
			"effect": "Deal 6 additional damage. Damage dealt by this ability is piercing damage."
		},
	],
	"flavor-text": "With a single strike it began, and with a single strike it ends.",
}
---
