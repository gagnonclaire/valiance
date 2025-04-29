---
{
	"name": "standard-melee-weapon",
	"tags": [ "equipment", "weapon", "ability" ],
	"tier": 0,
	"base-item": null,
	"primary-tag": {
		"tag": "action",
		"value": 1,
	},
	"secondary-tags": [
		{
			"tag": "attack",
			"value": 1,
			"value-max": null,
		},
		{
			"tag": "check",
			"value": null,
			"value-max": null,
		},
		{
			"tag": "range",
			"value": 1,
			"value-max": null,
		},
	],
	"energy-cost": 0,
	"effect": "Deal 4 damage.",
	"effect-trigger": null,
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
