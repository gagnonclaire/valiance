A status is a temporary effect that can be applied to a character during combat. Every status has a point value that determines its duration and intensity. An energized 3 would affect the character for the next three turns, with its effects diminishing over that time.

When a status is applied to a character that is already affected by that status, it instead adds its point value to the existing instance. For example, if a decaying 1 effect is applied to a character that already has decaying 2, the character will then be decaying 3. 

An the end of each of a character's turn, after applying any end of turn status effects, each of their statuses has one point cleared. When a status has 0 points it is removed from the character. This end of  decrease happens after any end of turn status effects. 

Status immunities prevent a certain status or statuses from being applied to the character with the immunity. When a character gains a status immunity while they have that status, the status is immediately cleared.
#### Boons
Positive statuses, usually applied to yourself or allies. Some boons allow their points to be spent, granting powerful effects and clearing the spent points. These statuses still have a point cleared at the end of the character's turn.

```dataview 
TABLE effect as "Effect"
FROM #boon
SORT file.name ASC
```
#### Ailments
Negative statuses, usually applied to your enemies.

```dataview 
TABLE effect as "Effect"
FROM #ailment
SORT file.name ASC
```