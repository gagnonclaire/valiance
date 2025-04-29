---
{
	"name": "heavy-melee-weapon",
	"tags": [ "equipment", "weapon", "ability" ],
	"tier": 0,
	"base-item": null,
	"primary-tag": {
		"tag": "action",
		"value": 2,
	},
	"secondary-tags": [
		{
			"tag": "attack",
			"value": 2,
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
	"effect": "Deal 6 damage.",
	"effect-trigger": null,
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
