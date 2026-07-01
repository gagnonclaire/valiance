Gear that makes you take piercing damage then empowers you. Clears the status when your guts are restored. Damage for half of current guts. Limited x gear
Continue to remove dependence on inter-character synergies
Clean up contracts section

Clean up all of the first few chapters
All function, no bullshit, if they want flavor they can read the archives

greatly simplify action resolution
standardize reactions

lot of things currently that are reaction but should be passive traits

No penalties for losing Valiance on a contract

Afflictions are individual disadvantages?
Should adv/disadv be team wide?

tiles with the breakable tag can be broken by targeting with any attack ability or an interact ability
if it's a tile face that target must be a tile that shares the face
breakable: this tile or a face connected to this tile may be broken
Archetype revision

Don't group archetypes under the three, they can all be their own
Move most pools into a common feats system
Allow multiclassing through the use of a repeatedly selectable feat (follows current rules for archetype restrictions)

recover, reaction 0, when your turn begins, end your turn and clear one of your ailments

allows the exists until removed ailment system without the weirdness of being caught out and staggered or something
also remove most cases of ailments that cam be cleared in nonstandard ways
rename grab cause it's not really a grab

hold?, stagger the target  if you are no longer adjacent to the target clear this ailment

Conditions for enemy character surrendering, like when they are staggered with no way out. Can be accepted by the party to speed up combat and save resources, or denied for fun

Mark mechanic
character target abilities can only target a marked character as long as the user can see a marked character
character vs tile target
like it sounds, abilities defined 'target character' or 'target tile'
damage dealt to tiles is dealt to characters on that tile
allow multihit for big characters?
target: character
target: self
target: tile
(etc.)

use hit points instead of stamina, energy point instead of energy
in general things that have current or variable values (hit points, damage points, etc.) are referred to as points

Strategies are used per round kinda like stances
Should they just be stances? Could balance them cause you couldn't use both
Strategies wouldn't be able to just be bonus shit, have to actually think about them and if a stance might be better

Make stances more general, changes gameplay round by round
Enemy characters shouldn't be able to use stances or transforms (rename transformation)?
Yeah that makes the gm job much easier, missing enemy stuff feels bad

buildups
critical meter

Enemy rework:
Instead of enemy characters have groups and actors that can fit neatly on an encounter sheet
Abstract, much more than players
Resources shared across team to simplify
Act as one to speed up enemy turns
power of abilities based on group, one member in range means all are when they use abilities
Group traits and abilities that each member of a group has access to
Individual members of a group then have their unique traits/abilities (usually only one or two)
Turns based on groups, with the players being one of the groups? Or each player controls a group consisting of themselves and any of their allies (make allies more prominent? Like a company resource? They would play them in combat though gm would roleplay them, maybe reject insane orders)
Group has defined reinforcements, specific member units that are good for continued pressure without being too oppressively (usually the more generic units of the group)
Keep unit type designations, have to rework turns and ability economy. Probably make resources group wide and elites/bosses have some special thing
group stun effect that skips the group's next turn
Turns taken in groups? As in all members of a group act simultaneously. Could work well with shared group resources such as available actions

Rename instant movement to be less cumbersome
field notes is a company resource?
All statuses are stacking, -1 stack at end of turn

rather than boosts use an advantage/fortune system? Like with adv 2 you roll 5d6 instead of 3d6 and take the 3 highest. Would alter the odds in a funny nonlinear way

targets:
character - any character within range
area - any character occupying the target tiles
self - the character that used the ability

no "multiple sources of abilities" stuff, if you have two of the same ability you can still only use it once per turn. Two weapon fighting allows you to stack traits and mix and match other effects instead

Effects conditional on status
"do x to an energized character"
"do y to an energized 4 or higher character"
"do z to an energized 3 or lower character"
Can be used to impose soft caps on statuses, punish status stacking (by players or enemies), allow use of statuses as a resource ("")

Trait: The Save ability clears an additional point of the selected status

types of movement:
move (standard)
shift (instantaneous)
forced (self-explanatory)

"secondary_value": 1, # not technically needed, if we have no secondary we just assume it's the same as primary (for range property)

In code, we have "ability" objects that hold functions based on name. For example, we have a "save" object that inherits the "ability" prototype object and implements its "on_use" function. The "on_use" function would probably take a "user" and "target" parameter along with an "options" and then do its thing. In this case, it would check usage validity based on the user and target, then look at the options param to determine which ailment to reduce.

Have error handling (vs hard crash) for:

- no user (every ability needs a user)
- no target (some abilities are exempt, such as strategies that affect the whole field)
- required options not found

May be some better way to store this game data, or even to generate it? Want to keep the ability to have all necessary pieces readable externally so we can gen rule docs with it.

penalty based fail system
out of combat encounters, have x rolls to resolve the encounter (resolving takes 1 or more success), every roll after that incurs a penalty for an upcoming scenario. until a certain number of penalties. At that point the party "fails" fully and must move on to the next scenario.
in combat, failing certain optional objectives might result in minor penalties. Failing a main objective would end the encounter (and downed characters lose a valiance point) and incur a major penalty, but not necessarily end the contract
pulling out of a contract early results in longer term penalties, such as a penalty applied to all future contracts until it is somehow resolved in or out of combat. Some penalties may be outline within the contract
failing to complete a contract means the team must regroup and eventually take on a different contract of the same tier, though they retain any rewards they obtained during the missions, such as smaller benefits obtained through secondary objectives (all resources dedicated to that contract are always lost, whether or not they were used by the time it fails or completes)


some system of direct hits where you roll 1d6 to determine if you go down, but you can always take at least 1. also direct hits reduce movement by 1? but can't reduce below 1.

maybe roll x d6, where x is the number of direct hits taken this combat

if >6, you go down

could technically limp along for several, but odds are you go down on the second

(you wouldn't roll the first one ever though since you can't get over 6 with one die)

maybe just a check (3d6), outcome determines effect

take a -1 penalty for each time rolled good: live with -1 move great: live perfect: live and don't take a penalty for this time

valiant trait where first direct hit would be a "close call", basically don't roll death and no penalty buildup

ultra enemies use the same system but no close call



elite enemies die on direct hit

normal enemies have half hp compared to elite

enemies don't use ep or limited

get rid of recharge

minimize things that need to be tracked

make complexity elsewhere



procurement point and wealth levels procurement points are used to procure equipment for your stash. A character starts with some procurement points and gains additional points at each tier up. wealth score is used for multiple things:
    
    determines which equipment items are unlocked for purchase with procurement points.
    determines the general wealth and affordable lifestyle of the character.
    unlocks amenities and services, such as a garage it workshop, that provide boosts for out of combat tools and items.
    
    maybe have some other personal points for acquiring nom combat tools. company resources used for various consumable boosts on mission, are acquired via a shared company resource pool. players cannot begin a contract while they have unused procurement points. items can be returned and replaced by any item of lower wealth tier (not equal, will always downgrade to make sure choices matter)
    
just use straight money for non equipment items? can exchange one way from procurement points to money based on the current wealth tier
    
or no wealth tier, and it's all just tied with tier
    
also all equipment just costs 1 point? start with 3 and gain 1 every tier up, with extra points available as bonus rewards (for the tier attained after completing that contract)


gameplay cycles based on seasons. contracts are short and do not span seasons. downtimes between contracts last one season per cycle, usually with two seasons (and downtimes) between contracts some costs are incurred for each downtime, such as rent for players renting housing or spaces. this is handled as an "upkeep cost" and also includes general upkeep for things the players use. this is all handled via money, with making money being a downtime activity (in addition to that made on contracts or by trading in procurement points)

valiance downtime a free downtime activity "catch up". the player selects one or more other characters (pc or npc) and a location and/or activity. the chosen characters play an encounter primarily driven by the character using the downtime. useful for checking in with each other and taking some time away from the narrative to develop characters and relationships. can be done once per downtime (season), but a character can be involved in multiple scenes (can only initiate one). highly encouraged, director will ask each player for their catch up (opt out, basically) by default, each catch up grants the initiating character one contingency point. other benefits, including other game resources, can be awarded by director discretion. encounter: a narrative or battle event that plays out in a single location, usually with on primary focus. game resource: any defined thing that can influence narrative or battle, like an item or an advantage. contingency point: used at any time (combat or narrative) to reroll a check. must take the new roll. the director must block this reroll (points are not used) if the result is the best possible outcome (ie the result is good and there are no great or perfect outcomes)