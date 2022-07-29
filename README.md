#  Crafting Handbook
  
## Table of Contents
* [Fundamentals of Crafting](https://github.com/RenTed87/Crafting_Handbook/blob/main/README.md#fundamentals-of-crafting)
* [Required Level (rlvl)](https://github.com/RenTed87/Crafting_Handbook/blob/main/README.md#required-level-rlvl)
* [Affix Level (alvl)](https://github.com/RenTed87/Crafting_Handbook/blob/main/README.md#affix-level-alvl)
* [General Tips](https://github.com/RenTed87/Crafting_Handbook/blob/main/README.md#general-tips)
* Amulets
* Rings
* [Gloves](https://github.com/RenTed87/Crafting_Handbook/blob/main/README.md#gloves)
* [Belts](https://github.com/RenTed87/Crafting_Handbook/blob/main/README.md#belts)
* [Boots](https://github.com/RenTed87/Crafting_Handbook/blob/main/README.md#boots)
* [Appendix](https://github.com/RenTed87/Crafting_Handbook/blob/main/README.md#appendix)
  
## Fundamentals of Crafting
### Level Terms
To keep track of the various levels involved, we will be making frequent use of these abbreviations,
  
* alvl - affix level of the crafted item; see the Affix Level (alvl) section
* Alvl - area level; relevant if using magic items from chests, racks etc. as craft supplies
* clvl - character level, in this case the level of the character which is gambling, shopping, or crafting
* ilvl - internal level of magic item; the "input item level"
* Ilvl - internal level of crafted item; the "output item level"
* mlvl - monster level; if using magic items from monsters as craft supplies, remember that ilvl = mlvl
* qlvl - base item Quality Level: http://classic.battle.net/diablo2exp/items/weaponsandarmor.shtml
* rlvl - required level; see the Required Level (rlvl) section
  
### Crafted Items at the Arreat Summit
http://classic.battle.net/diablo2exp/items/crafteditems.shtml  
Sufficient if you do not mind not knowing every single detail.
  
### Craft Recipes
As of now there are 4 classes of crafted items, each containing 9 recipes (see the Arreat Summit Crafted Items page),
* Magic Item (specific type) + Rune (specific) + Perfect Sapphire + Jewel --> Hit Power Item (of the same type)
* Magic Item (specific type) + Rune (specific) + Perfect Ruby + Jewel --> Blood Item (of the same type)
* Magic Item (specific type) + Rune (specific) + Perfect Amethyst + Jewel --> Caster Item (of the same type)
* Magic Item (specific type) + Rune (specific) + Perfect Emerald + Jewel --> Safety Item (of the same type)
  
Listen very carefully; I shall say this only once,
    -The properties of the Magic Item are LOST when the crafted item is generated.
    -ANY Jewel works (magic, rare, unique) and the Jewel has NO impact on the result.
    -Ethereal (transparent) magic items will be turned into opaque (not transparent) crafted items, because the Horadric Cube is used to generate a completely new item.
  
Due to the plethora of rare, set, and unique items, and rune words, most craft recipes aren't worth the trouble. It is the fact that some desired modifiers can only spawn together on crafted items which makes them competitive. By virtue of possessing both fixed properties and random affixes (prefixes, suffixes), crafted items are able to get as much as 7 or 8 modifiers.  
  
### Popular Crafts
* Caster Amulet
* Safety Amulet
* Blood Ring
* Hit Power Gloves
* Blood Gloves
* Blood Belt
* Caster Belt
* Caster Boots
  
Seeing how the same concepts transfer to every other craft recipe, the remaining sections should enable you to work out how to craft efficiently, no matter the recipe.  
  
### Fixed Properties
A crafted item receives either 3 or 4 fixed properties, depending on and invariably set by the recipe, and spawning at one of the values listed, picked at random.  
  
### Random Affixes
On top of the fixed properties, a crafted item receives 1-4 random affixes, depending on Ilvl,
* Ilvls 1-30: 4 affixes (20 %), 3 affixes (20 %), 2 affixes (20 %), 1 affix (40 %)
* Ilvls 31-50: 4 affixes (20 %), 3 affixes (20 %), 2 affixes (60 %)
* Ilvls 51-70: 4 affixes (20 %), 3 affixes (80 %)
* Ilvls 71+: 4 affixes (100 %)
  
**Notice**  
The random affixes that spawn on crafted items are picked from the list of affixes available on rare items of the same type. Magic-only affixes cannot spawn.
  
Meaning, the affix generation rules for rare items transfer to crafted items: max 3 prefixes and max 3 suffixes from distinct affix groups. Thus, 4 affixes spawn as either 1/3, 2/2, or 3/1 prefixes/suffixes (never 0/4 or 4/0) and no two of these can belong in the same group. Usually not a serious restriction but nonetheless one worth remembering, as it explains what affix combinations we can possibly craft.
  
Some fixed properties and random affixes are two of a kind, perhaps with different values. Example: since a rare Amulet has +10 % FCR or none (there is only one FCR suffix for Amulets), a Caster Amulet with its fixed property: +5-10 % FCR will always have at least +5-10 % FCR and may get +15-20 % FCR. Other examples of stackable fixed properties and random affixes include: Life, Mana, Strength, and Dexterity. Hence, a Caster Amulet could get up to +110 to Mana (fixed property: +10-20 to Mana and up to +90 to Mana from the prefix, "Great Wyrm's").
  
### The "output item level" (Ilvl)  
You may have noticed how the Arreat Summit uses "ilvl" for both the magic and crafted item. Although the meaning should be clear to most of you, I cannot stress enough the importance of distinguishing between the two. They are different levels; the ilvl of the magic item to be crafted is used to calculate the Ilvl (capital I) of the crafted item,
  
    Ilvl = int(clvl/2) + int(ilvl/2)
  
Evidently, clvl and ilvl are equally important when crafting. For those who are not familiar with the integer part,
  
     int(n/2) =  n/2     ,  if n is even
     int(n/2) = (n-1)/2  ,  if n is odd
  
The above formula for the Ilvl is the backbone of crafting. Without knowing it, we would all be 'blindcrafting', not having the faintest idea if the desired affixes could spawn, or the resulting Ilvl is too low. Conversely, if the Ilvl is higher than necessary, we run the risk of rolling higher, potentially unwanted affixes which we might avoid if we had known what clvl and ilvl to use.
  
## Required Level (rlvl)
  
The required level of an item is the minimum character level that may use it. For crafted items,
  
     rlvl = rlvl_affix + 10 + 3*N ;  capped at 98
  
where rlvl_affix is the highest levelreq amongst the random affixes that spawned, and N is the number of random affixes (1, 2, 3, or 4).
  
Example: a crafted Amulet with 4 random affixes and +2 to [class] skills having the highest levelreq (rlvl_affix = 67) will have rlvl = 67 + 10 + 3*4 = 89. Pre-1.11, certain charged affixes could force the rlvl beyond 99 (nice move, Blizzard); this was remedied in v1.11: if rlvl > 98, then rlvl = 98. Despite this, in certain cases the rlvl formula is still of some concern.
  
## Affix Level (alvl)
  
When an item with affixes is generated, the game calculates the item's affix level (alvl), as described below. Then it looks up the affixes available for that item type and affix level. Every affix has a level, the minimum alvl which must be met by an item of the proper type to acquire that affix. Higher alvl ~ larger affix pool. For a crafted item, 1-4 affixes are picked according to Ilvl and affix generation rules. Due to differences in affix frequencies, some affixes are slightly more likely to spawn than others. Players who have installed ATMA may find detailed information on every single affix in MagicPrefix.txt and MagicSuffix.txt.
  
* The affix level of a crafted item is of crucial importance, because it effectively determines the size of the affix pool.
* When looking at affixes, we have to consider: level, levelreq, and group (it is impossible to get more than one affix from a given group).
  
**Affix Level Calculation**
  
     IF(magiclvl > 0)
        (1) THEN alvl = max{Ilvl,qlvl} + magiclvl
     ELSE IF(max{Ilvl,qlvl} < 99 - int(qlvl/2))
        (2) THEN alvl = max{Ilvl,qlvl} - int(qlvl/2)
        (3) ELSE alvl = 2*max{Ilvl,qlvl} - 99
  
Ilvl cannot exceed 98 (see the Ilvl formula) and alvl is capped at 99
  
Only Circlets, Sorceress Orbs, Staves, and Normal + Exceptional Wands have magiclvl > 0. However, there are no craft recipes for Circlets and Orbs, and rather few players would craft Staves or Wands, seeing as the unique versions and rune words are practically beyond competition.
  
Consult the Arreat Summit for qlvl (and magiclvl),
  
* http://classic.battle.net/diablo2exp/items/ringsnamulets.shtml
* http://classic.battle.net/diablo2exp/items/weaponsandarmor.shtml
  
Notice: Amulets and Rings have qlvl 1.
  
**The Broad Picture**  
For a given base item (qlvl), alvl is effectively determined by Ilvl, which in turn is given by the previous formula: Ilvl = int(clvl/2) + int(ilvl/2). See Appendix for a compact Ilvl table based on gambling / shopping and crafting magic items. If we can find suitable clvl and ilvl so that the alvl is at least equal to the highest level amongst the affixes we desire, then we always have a chance of rolling that affix as well as any affixes with a lower level.
  
Crafting efficiently is thus a matter of using the affix level formulae to our advantage,
  
    We pick a craft recipe and look up the qlvl(s).
    For Staves and Wands (not Elite Wands), we use (1).
    For other base items, we consider max{Ilvl,qlvl} < 99 - int(qlvl/2),
       a) Assuming this is true, from (2) we get the minimum Ilvl required for the desired alvl.
       b) Otherwise, we use (3) in a similar manner.
    Turning to the Ilvl formula, we work out suitable values of clvl and ilvl.
  
Now, before we immerse ourselves in numbers and calculations, but first, some advice on gathering craft material...
  
## General Tips
Crafting is entirely straightforward if we do not care about the details, but without the requisite information at hand, it may just as well be a complete waste of resources. Since the odds of crafting what you want are usually quite low already, you could at least do yourself a favour by ensuring that bad luck is the only reason you have to craft repeatedly.
  
**Checklist**
* Know what you want; which modifiers do you desire ? Check if they can possibly spawn on that type of item.
* Look up level, levelreq, and group for each affix: https://planetdiablo.eu/diablo2/itemdb/affix_index.php?lang=en&version=lod&patch=111
* Always check that the Ilvl, and hence the alvl, of the craft will be sufficiently large to generate the higher level affix.
* Run the higher levelreq and number of random affixes in the rlvl formula if the required level is of any concern.
  
Alright, but where do we quickly gather magic items for crafting ? And how is the ilvl determined ?
  
**Gambling**
* http://classic.battle.net/diablo2exp/basics/gambling.shtml
  
Notice: only character level matters when gambling. Formally,
  
    ilvl = clvl - 5 + rnd(10) ;  capped below at 5 and above at 99
  
Where rnd(10) returns a random integer from 0 to 9. Thus, the gambled ilvl ranges from clvl - 5 to clvl - 5 + 9 = clvl + 4. That being said, it pays to gamble in Hell, because the partial refund (up to 35 k Gold) is greater than in Normal (up to 5, 10, 15, 20, 25 k Gold, depending on Act) and Nightmare (up to 30 k Gold).
  
**Shopping**  
As opposed to gambling, the ilvl when shopping is not subject to random behaviour,
  
     ilvl = clvl + 5 ;  capped at 99, further restricted in Normal by Act (see the NPC Shopping Calculator)
  
Certain items cannot be shopped, notably Amulets and Rings. They must be either gambled or retrieved as item drops.
  
**Vendor Discount**
* Gheed's Fortune (Grand Charm), Ladder Only: Reduces All Vendor Prices 10-15 %
* Edge ('TirTalAmn'), miss, Ladder Only: Reduces All Vendor Prices 15 %
  
Thus, a potential discount of 25-30 % when gambling or shopping.
  
**Magic Item Drops**  
Relying on these as your only craft material is not recommended unless you cannot gamble or shop the base items (e.g. Amazon Javelins and Spears). Nor is this an instruction to throw away every magic item with junk properties just because the item type could be gambled or shopped. If the ilvl of a magic item drop is sufficiently high for crafting, then keep it for that purpose. As a quick reference,
  
    ilvl = mlvl (monster drops)
    ilvl = Alvl (chest drops)
    ilvl = Alvl - 1 (rack drops)
    mlvl = Alvl (regular monsters)
    mlvl = Alvl + 2 (champions, any kind)
    mlvl = Alvl + 3 (bosses and minions)
  
The mlvl-Alvl relations hold for Nightmare and Hell. Monsters in Normal difficulty use mlvls defined in MonStats.txt. Check the Diablo II Resources section of my profile for Area Levels.
  
## Amulets
### Random Affixes
**Desired:**
* (P) "Great Wyrm's" (level 37, levelreq 29, group 115): +61-90 to Mana
* (P) "Prismatic" (level 42, levelreq 31, group 116): All Resistances +16-20
* (P) "Sapphire/Ruby/Amber/Emerald" (level 25, levelreq 18, group 117/118/119/120): Cold/Fire/Lightning/Poison Resist +31-40 %
* (P) "[class dependent]" (level 90, levelreq 67, group 125): +2 to [class] Skill Levels / Skills
* (S) "of the Apprentice" (level 5, levelreq 3, group 9): +10 % FCR
* (S) "of Perfection" (level 59, levelreq 51, group 17): +16-20 to Dexterity
* (S) "of the Colossus" (level 30, levelreq 22, group 26): +41-60 to Life
* (S) "of Atlas" (level 71, levelreq 63, group 31): +21-30 to Strength
  
The highest level amongst these is 90 (+2 to [class] Skill Levels / Skills), so we have to ensure that alvl >= 90. From then on, crafting is purely a matter of luck; any Amulet affix with level 90 or less is able to spawn (which is, in fact, any Amulet affix) and there is no way we can rule out lower affixes.
  
### Optimised Crafting
Amulets have qlvl 1, implying max{Ilvl,qlvl} = Ilvl. So, if Ilvl < 99 - int(1/2) = 99, we use (2). Since this is always the case (Ilvl cannot exceed 98), we get alvl = Ilvl. Thus, we need at least Ilvl 90,
  
    int(clvl/2) + int(ilvl/2) >= 90.
  
Gambling is the quickest. Now, ilvl = clvl - 5 + rnd(10). Here, we pick the worst case scenario: ilvl = clvl - 5 and plug this into the above condition,
  
    int(clvl/2) + int((clvl - 5)/2) >= 90
  
Yielding clvl >= 93 (check it !). So, the conclusion is,
  
* **Use a character of at least level 93 to gamble and craft Amulets - then every Amulet has a chance to get +2 to [class] Skill Levels / Skills.**
  
Because 93 - 5 = 88, any ilvl 88+ Amulet will suffice. That is, magic Amulets dropped from bosses and minions in Alvl 85 or from Hell Diablo, Nihlathak, and Baal work as well.
  
_How about the rlvl ? We know it will be 89 if +2 to [class] Skill Levels / Skills is the affix having the highest levelreq (67). However, there are two Amulet suffixes with levelreq > 67, viz, "of the Lamprey" (levelreq 73): 6 % Life Stolen Per Hit, and "of Bone Spirit" (levelreq 72): Level 1 Bone Spirit charges. Due to these, we may occasionally be looking at rlvl 95 or rlvl 94._
  
## Rings
### Random Affixes
**Desired:**
* (P) "Platinum" (level 22, levelreq 16, group 110): +101-120 to AR
* (P) "Great Wyrm's" (level 37, levelreq 29, group 115): +61-90 to Mana
* (P) "Rainbow" (level 56, levelreq 48, group 116): All Resistances +8-11
* (P) "Cobalt/Garnet/Coral/Jade" (level 18, levelreq 13, group 117/118/119/120): Cold/Fire/Lightning/Poison Resist +21-30 %
* (S) "of the Apprentice" (level 5, levelreq 3, group 9): +10 % FCR
* (S) "of Precision" (level 56, levelreq 48, group 17): +10-15 to Dexterity
* (S) "of the Mammoth" (level 68, levelreq 60, group 26): +31-40 to Life
* (S) "of the Lamprey" (level 77, levelreq 65, group 27): 7-8 % Life Stolen Per Hit
* (S) "of the Vampire" (level 86, levelreq 74, group 28): 6 % Mana Stolen Per Hit
* (S) "of the Titan" (level 74, levelreq 66, group 31): +16-20 to Strength
  
Although the highest level is 86 (6 % Mana Stolen Per Hit), we do not necessarily want to push the alvl that far, seeing how it may result in rlvl 96 (74 + 10 + 3*4). In order to circumvent this and still be able to roll the other affixes, our target alvl should be at least 77 and at most 85.
  
### Optimised Crafting
Rings have qlvl 1, just like Amulets. Thus, we need at least Ilvl 77 and at most Ilvl 85,
  
    76 < int(clvl/2) + int(ilvl/2) < 86
  
Again, the efficient approach is Gambling. However, with the addition of an upper bound (Ilvl < 86), this time we cannot just pick ilvl = clvl - 5 and be content with that. We must check the other extreme as well: ilvl = clvl + 4,
  
    76 < int(clvl/2) + int((clvl - 5)/2) < 86
    76 < int(clvl/2) + int((clvl + 4)/2) < 86
  
Solving these simultaneously yields 79 < clvl < 84. That is,
  
* **Whenever rlvl 96 is of any concern, use a level 80-83 character to gamble and craft Rings.**
  
_Conversely, if we want every Ring to have a chance of acquiring 6 % Mana Stolen Per Hit, we should use a character of at least level 89, in which case we might occasionally be looking at rlvl 96. If we use a level 80-83 character to gamble and craft, then at most rlvl 88 ("of the Titan": levelreq = 66)._
  
## Gloves  
### Random Affixes
**Desired:**
* (P) "Cobalt/Garnet/Coral/Jade" (level 18, levelreq 13, group 117/118/119/120): Cold/Fire/Lightning/Poison Resist +21-30 %
* (P) "Bowyer's/Gymnastic/Spearmaiden's" (level 40, levelreq 30, group 125): +2 to Bow and Crossbow/Passive and Magic/Javelin and Spear Skills (Amazon Only)
* (S) "of Alacrity" (level 43, levelreq 35, group 7): +20 % IAS
* (S) "of Precision" (level 56, levelreq 48, group 17): +10-15 to Dexterity
* (S) "of the Giant" (level 59, levelreq 51, group 31): +10-15 to Strength
  
**Unwanted:**
* (S) "of Weaken" (level 24, levelreq 24, group 44): Level 5 Weaken charges
* (S) "of Power Strike" (level 55, levelreq 47, group 44): Level 4 Power Strike charges
* (S) "of Multiple Shot" (level 63, levelreq 55, group 44): Level 4 Multiple Shot charges
* (S) "of Charged Strike" (level 68, levelreq 60, group 44): Level 3 Charged Strike charges
* (S) "of Freezing Arrow" (level 94, levelreq 86, group 44): Level 2 Freezing Arrow charges
  
Note that we cannot rule out the 6 charged suffixes with level < 59, because we want a chance to hit the suffix, "of the Giant". But we will try to freeze out as many of the 7 higher charged suffixes as possible. The charged suffixes available on gloves are basically useless and the highest ones increase the rlvl a LOT. You will probably not be pleased with your 'kick-ass' crafted gloves if they require level 98.
  
Looking at the above values, our initial target alvl would be at least 59 and at most 62.
  
### Hit Power Gloves  
Chain Gloves (qlvl 12), Heavy Bracers (qlvl 43), Vambraces (qlvl 69). In each case, we consider max{Ilvl,qlvl} < 99 - int(qlvl/2).
  
**Chain Gloves**  
max{Ilvl,12} < 99 - int(12/2) = 93 <=> Ilvl < 93. Suppose this is the case. From (2), 58 < max{Ilvl,12} - 6 < 63 <=> 64 < Ilvl < 69. Notice the problem here; Ilvls 51-70: 4 affixes (20 %), 3 affixes (80 %). Only every 5th pair of gloves would get 4 affixes, on average. Since we want 4 affixes, we have to compromise. Ilvl 71-73 (alvl 65-67) would guarantee 4 affixes and still eliminate 6 of the 7 higher charged suffixes (only "of Multiple Shot" has 59 < level < 68). Plugging this into the Ilvl formula,
  
    70 < int(clvl/2) + int(ilvl/2) < 74
  
Similar to the restriction imposed on the Rings, but now the Ilvl range is thrice as narrow. If we gamble, ilvl = clvl - 5 yields 73 < clvl < 77, whereas ilvl = clvl + 4 yields 69 < clvl < 72. No single clvl is able to cover both extremes. But we have another option: Shopping. This would fix the ilvl at clvl + 5 and hence,
  
    70 < int(clvl/2) + int((clvl + 5)/2) < 74
  
from which 68 < clvl < 72. Use the NPC Shopping Calculator to get a suitable vendor selling Chain Gloves.
  
**Heavy Bracers**  
max{Ilvl,43} < 99 - int(43/2) = 78 <=> Ilvl < 78. Suppose this is true. Then, from (2), 58 < max{Ilvl,43} - 21 < 63 <=> 79 < Ilvl < 84, contradicting Ilvl < 78. So, we must have Ilvl >= 78 and from (3), 58 < 2*max{Ilvl,43} - 99 < 63 <=> 78 < Ilvl < 81. Plugging this into the Ilvl formula and assuming we shop the gloves,
  
    78 < int(clvl/2) + int((clvl + 5)/2) < 81
  
yielding 76 < clvl < 79. Use the NPC Shopping Calculator to determine who can sell Heavy Bracers.
  
**Vambraces**  
Cannot be shopped, so we skip the calculations. Good luck gambling Vambraces, or getting them to drop, with the proper ilvl, quickly enough to compete with the other types.
  
### Blood Gloves  
Heavy Gloves (qlvl 7), Sharkskin Gloves (qlvl 39), Vampirebone Gloves (qlvl 63). Same procedure as last recipe, Darling ? Same procedure as every recipe, n00b.
  
**Heavy Gloves**  
70 < Ilvl < 75 (67 < alvl < 72; only the 4 highest charged suffixes (level 72+) frozen out). Shopping Heavy Gloves, 68 < clvl < 73.
  
**Sharkskin Gloves**  
77 < Ilvl < 80 (58 < alvl < 61; the 7 highest charged suffixes (level 61+) frozen out). Shopping Sharkskin Gloves, 75 < clvl < 78.
  
**Vampirebone Gloves**  
Cannot be shopped.
  
**Summary:**
* Use a level 69-71 character to shop Chain Gloves and craft them, using the Hit Power Gloves recipe.
* Use a level 77-78 character to shop Heavy Bracers and craft them, using the Hit Power Gloves recipe.
* Use a level 69-72 character to shop Heavy Gloves and craft them, using the Blood Gloves recipe.
* Use a level 76-77 character to shop Sharkskin Gloves and craft them, using the Blood Gloves recipe.
  
_The Chain Gloves will have at most rlvl 77 ("of Multiple Shot": levelreq = 55) while freezing out the 6 highest charged suffixes. Both Heavy Bracers and Sharkskin Gloves are unable to get any of the 7 highest charged suffixes and should thus not exceed rlvl 73 ("of the Giant": levelreq = 51). And the Heavy Gloves, blocking the 4 highest charged suffixes from spawning, are limited to no more than rlvl 83 ("of Exploding Arrow": levelreq = 61)._

## Belts
### Random Affixes
**Desired:**
* (P) "Serpent's" (level 14, levelreq 10, group 115): +11-20 to Mana
* (P) "Cobalt/Garnet/Coral/Jade" (level 18, levelreq 13, group 117/118/119/120): Cold/Fire/Lightning/Poison Resist +21-30 %
* (S) "of Stability" (level 18, levelreq 13, group 18): +24 % FHR
* (S) "of the Colossus" (level 30, levelreq 22, group 26): +41-60 to Life
* (S) "of Atlas" (level 71, levelreq 63, group 31): +21-30 to Strength
  
Highest amongst these: level 71, so we need at least alvl 71 when crafting. Only Blood Belt and Caster Belt will be covered here; the other belt recipes are rarely used. In want of brevity, we head straight to the results.
  
### Blood Belt
Belt (qlvl 12), Mesh Belt (qlvl 43), Mithril Coil (qlvl 75).
  
### Caster Belt
Light Belt (qlvl 7), Sharkskin Belt (qlvl 39), Vampirefang Belt (qlvl 68).
  
Maximum efficiency and to avoid having to use multiple characters,
  
* **Use a character of at least level 88 to gamble or shop the above belts and craft them, using the Blood Belt or Caster Belt recipes.**
  
Gamble in Hell or use the NPC Shopping Calculator to work out which vendors can sell Belt, Mesh Belt, Light Belt, and Sharkskin Belt, respectively. Mithril Coil and Vampirefang Belt cannot be shopped.
  
_At most rlvl 85 ("of Atlas": levelreq = 63)._
  
## Boots
### Random Affixes
**Desired:**
* (P) "Dragon's" (level 52, levelreq 39, group 115): +31-40 to Mana
* (P) "Sapphire/Ruby/Amber/Emerald" (level 25, levelreq 18, group 117/118/119/120): Cold/Fire/Lightning/Poison Resist +31-40 %
* (S) "of Accuracy" (level 46, levelreq 38, group 17): +6-9 to Dexterity
* (S) "of Balance" (level 5, levelreq 3, group 18): +10 % FHR
* (S) "of Regeneration" (level 70, levelreq 52, group 19): Replenish Life +3-5
* (S) "of Speed" (level 37, levelreq 29, group 35): +30 % FR/W
  
Although most of the above boot affixes are desired regardless, we are mainly concerned with the popular Caster Boots, hence the inclusion of the "Dragon's" prefix. Again, leaving out the calculations.
  
### Caster Boots
Boots (qlvl 3), Demonhide Boots (qlvl 36), Wyrmhide Boots (qlvl 60).
  
Maximum efficiency and to avoid having to use multiple characters,
  
* **Use a character of at least level 88 to gamble or shop the above boots and craft them, using the Caster Boots recipe.**
  
Adjust the character level accordingly if you prefer not rolling the suffix, "of Regeneration". By now, you should know how to achieve this.
  
_At most rlvl 74 ("of Regeneration": levelreq = 52)._
  
## Appendix
The table lists character levels granting the crafted item at least 1, 2, 3, or 4 random affixes.
  
    Magic craft supplies gambled or shopped at NPCs and subsequently crafted
  
    Gambled items: ilvl = clvl - 5 + rnd(10). Shopped items: ilvl = clvl + 5
  
                        Ilvl = int(clvl/2) + int(ilvl/2)
  
  
                             Gambling  +  Crafting
  
     clvl *)         Ilvl        1 affix    2 affixes    3 affixes    4 affixes
  
     1-29            1-30          40 %        20 %         20 %         20 %
    34-49           31-50                      60 %         20 %         20 %
    54-69           51-70                                   80 %         20 %
    74-99           71+                                                 100 %
  
  
                             Shopping  +  Crafting
  
     clvl            Ilvl        1 affix    2 affixes    3 affixes    4 affixes
  
     1-28            1-30          40 %        20 %         20 %         20 %
    29-48           31-50                      60 %         20 %         20 %
    49-68           51-70                                   80 %         20 %
    69-99           71+                                                 100 %
  
_Character level range corresponding to Ilvl range, regardless of gambled ilvl, e.g. clvl 34 guarantees at least Ilvl 31,
thereby excluding the possibility of 1 affix on the craft, while clvl 49 corresponds to at most Ilvl 50 (ilvl 52 or 53)._
  
_Character levels not listed are not recommended; corresponding Ilvls would be distributed over two of the given intervals._
