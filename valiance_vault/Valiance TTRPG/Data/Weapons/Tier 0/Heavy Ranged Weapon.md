---
{
	"name": "heavy-ranged-weapon",
	"tags": [ "equipment", "weapon", "ability" ],
	"tier": 0,
	"target": character,
	"energy-cost": 0,
	"properties": [
		"action 2",
		"attack 2",
		"check",
		"range 1-6",
	],
	"effect": "Deal 6 damage. This ability cannot be used while you are engaged.",
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
	"flavor-text": "One shot.",
}
---
