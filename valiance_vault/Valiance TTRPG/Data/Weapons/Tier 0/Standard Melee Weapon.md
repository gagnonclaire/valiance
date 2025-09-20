---
{
	"name": "standard-melee-weapon",
	"tags": [ "equipment", "weapon", "ability" ],
	"tier": 0,
	"target": character,
	"energy-cost": 0,
	"properties": [
		"action 1",
		"attack 1",
		"check",
		"range 1",
	],
	"effect": "Deal 4 damage.",
	"check-effects": [
		{
			"result": "good",
			"effect": "Deal 1 additional damage."
		},
		{
			"result": "great",
			"effect": "Deal 2 additional damage."
		},
		{
			"result": "perfect",
			"effect": "Deal 3 additional damage. Damage dealt by this ability is piercing damage."
		},
	],
	"flavor-text": "A strong arm, a sturdy grip, and a will to apply them.",
}
---
