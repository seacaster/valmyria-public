---
title: Living Rules Doc
date: \today
toc: true
numbersections: true
geometry: margin=0.5in
urlcolor: blue
---

[//]:
  #
  "To convert this to pdf, run:
cd C:\\Users\aqw20\DnD\Writeups
pandoc -o rules.pdf rules.md
To change wrapping, use the following Prettier commands.
Hard wrap at 80 characters: npx prettier rules.md --prose-wrap always --write
No wrap: npx prettier rules.md --prose-wrap never --write"

All published content is allowed, including optional subclasses/features/options
from Tasha’s.

# Character Mechanics

## Character Creation

- Standard point buy for stats (27 points, min 8, max 15)
- Any race (besides Variant Human and Custom Lineage) can take a feat at
  character creation in exchange for their racial ASI(s) becoming a single +1
- Players can assign racial ASIs to any stat, but cannot put multiple racial
  ASIs on the same stat (a la Tasha's)

## Leveling Up

- PCs get a free feat at levels 4 and 8 in addition to the ASIs at those levels

## Class Changes

### Monk

- Additional ki points equal to proficiency bonus
- If you are not wearing armor and not wielding a shield, enemy creatures have
  disadvantage on opportunity attacks against you
- Can make grapple/shove checks with DEX (Athletics)

### Sorcerer

- Additional metamagic options
  - 3 metamagic options at 3rd level
  - 4th option at 6th level
  - 5th and 6th at 10th and 17th level (as normal)
- 2 additional sorcery points
- All subclasses get origin spells (specific spells TBD)

### Warlock

- Warlocks can choose to use INT as their primary stat
  - CHA save proficiency becomes INT save proficiency
  - Spellcasting stat becomes INT
  - All class features that reference CHA will use INT instead

## Race Changes

- Dragonborn breath weapons are a bonus action, not an action

# Gameplay

## Resting

- Slow Natural Healing variant rule from DMG
  - Short rests are 1 hour; hit dice can be used to restore HP
  - Long rests are 8 hours; all resources are restored, and hit dice can be used
    to restore HP.
  - Can only benefit from 1 long rest every 24 hours

## Combat

### Flanking

- Prerequisites:
  - Two allied creatures, both directly adjacent to a hostile creature (but on
    opposite sides).
  - The allied creatures cannot be unconscious or incapacitated.
- Result: The allied creatures are **_flanking_** the hostile creature
  - While flanking, melee attacks get a +2 to hit

### Moving through enemy space

- A creature can do either of the following as an action or bonus action to move
  through enemy space.
  - _**Overrun**_: Make a contested STR (Athletics) check. Larger creatures have
    advantage.
  - _**Tumble**_: Make a contested DEX (Acrobatics) check.

### Cleaving and Piercing

- Cleaving (requires reducing an enemy to 0 HP with a melee weapon attack)
  - Any excess damage can be applied to another creature within reach
- Piercing (requires reducing an enemy to 0 HP with a ranged weapon attack)
  - Any excess damage can be applied to a creature 5 feet behind target
    (following straight line of projectile path)
- AC must be equal to or below the initial attack roll for both cleaving and
  piercing

### Identifying Spells

INT (Arcana) check when a spell is cast

- DC is 15 + spell level to identify specific spell, 10 + spell level to
  identify the level
- Consumes your **reaction**, but you _can_ cast Counterspell as part of the
  same reaction
- Advantage if the spell is on your spell list
- Disadvantage if you don't have Arcana proficiency
- Can't retry identifying a spell without getting more information

### Other Changes and Clarifications

- Potions require a bonus action to drink, not an action
- You cannot use both your action and your bonus action to cast spells of level
  1 or higher in the same turn.

# Workshop

Rules in this section are _not_ in current use - they're here for feedback and
possible future integration.

## Character Progression

A system to split ASIs from feats would be good to allow MAD classes to keep
statistical parity while still being able to take interesting feats.

**Proposed solution: +1 to an ability score and +1 feat point every even level**

### Ability Score Improvements

Giving a +1 to any ability score every 2 levels seems doable. This lets a MAD
class with a typical +2/+1 race go from 17/16/14 to 20/18/14 or 18/18/16 at
level 10. It's a bit of an accelerated power curve (easily accessible +4 primary
modifiers at level 2) but that's fine.

### Feats

- Feats will cost either 1 or 2 feat points.
- Half-feats cost 1 point and full feats cost 2.
- Half-feats no longer grant stat bonuses.
- Lucky is banned due to the generally low number of combats per long rest.

# Changelog

- 2/9/21: Initial version
  - Add rules from /u/Caesarr
    - Rules to take effect immediately:
      - Monk changes (additional ki, conditional disadvantage on opportunity
        attacks, grapple/shove with DEX)
      - Sorcerer changes (metamagics, additional SP, origin spells)
      - Warlock changes (INTlocks)
      - Cleave rules
  - Rules to take effect at next character creation:
    - Non-human races can give up their +2 ASI for a feat
- 2/16/21: Add flanking, wording/structure clarifications, move TODOs
  - Exhaustion on hitting 0 HP seems like a bad call
- 6/15/21: Redo spell ID rules
  - Random instead of deterministic
  - Allow people without proficiency to try (at disadvantage)
  - Consume reaction without preventing simultaneous counterspell
  - Make use of advantage/disadvantage less awkward
- 6/26/21
  - Allow spell ID arcana check to identify spell level (DC 10 + spell level)
  - Add character progression stuff to workshop

# TODOs

- Consider if sorcerer changes are overtuned given availability of feats (ease
  of taking Metamagic Adept)
- Consider boosted healing rules (spells/potions heal max or double dice if
  healing creature above 0 HP)
