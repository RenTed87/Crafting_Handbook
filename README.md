#  Crafting Handbook

## Table of Contents
* [Fundamentals of Crafting](https://github.com/RenTed87/Crafting_Handbook/edit/main/README.md#fundamentals-of-crafting)
* [Required Level (rlvl)](https://github.com/RenTed87/Crafting_Handbook/edit/main/README.md#required-level-rlvl)
* Affix Level (alvl)
* General Tips
* Amulets
* Rings
* Gloves
* Belts
* Boots
* Appendix

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
  
Ref: Things you SHOULD know about Diablo 2, section 23, http://classic.battle.net/forums/thread.aspx?fn=d2-general&t=1312543
  
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
  
Ref: Basin Wiki, D2 Affix Level Chart, http://wiki.theamazonbasin.com/index.php/D2_Affix_Level_Chart
  
Only Circlets, Sorceress Orbs, Staves, and Normal + Exceptional Wands have magiclvl > 0. However, there are no craft recipes for Circlets and Orbs, and rather few players would craft Staves or Wands, seeing as the unique versions and rune words are practically beyond competition.
  
Consult the Arreat Summit for qlvl (and magiclvl),

* http://classic.battle.net/diablo2exp/items/ringsnamulets.shtml
* http://classic.battle.net/diablo2exp/items/weaponsandarmor.shtml
  
Notice: Amulets and Rings have qlvl 1.
  
**The Broad Picture**  
For a given base item (qlvl), alvl is effectively determined by Ilvl, which in turn is given by the previous formula: Ilvl = int(clvl/2) + int(ilvl/2). See Appendix for a compact Ilvl table based on gambling / shopping and crafting magic items. If we can find suitable clvl and ilvl so that the alvl is at least equal to the highest level amongst the affixes we desire, then we always have a chance of rolling that affix as well as any affixes with a lower level.

Crafting efficiently is thus a matter of using the affix level formulae to our advantage,

* We pick a craft recipe and look up the qlvl(s).
* For Staves and Wands (not Elite Wands), we use (1).
* For other base items, we consider max{Ilvl,qlvl} < 99 - int(qlvl/2),
* a) Assuming this is true, from (2) we get the minimum Ilvl required for the desired alvl.
* b) Otherwise, we use (3) in a similar manner.
* Turning to the Ilvl formula, we work out suitable values of clvl and ilvl.

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
* http://members.iinet.net.au/~dcarson/shopcalc.html (NPC Shopping Calculator)
  
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
  
  
  
  
  
