---
{
	"name": "standard-ranged-weapon",
	"tags": [ "equipment", "weapons" ],
	"tier": 0,
	"base-weapon": null,
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
			"value-max": 4,
		},
	],
	"effect": "Deal 4 damage. This ability cannot be used while you are engaged.",
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
	"flavor-text": "She cleaned her fathers revolver and wondered, as she always did before a job, if this would be the last time.",
}
---
