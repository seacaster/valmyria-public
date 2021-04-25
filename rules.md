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

test change 6

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
  - 4 metamagic options at 3rd level
  - Another two at 10th level (up to 6)
  - Another two at 17th level
- Additional sorcery points equal to proficiency bonus
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

- Passive INT (Arcana) check
  - Advantage (passive +5) if spell is on spell list
  - Identify spell level with DC 10 + spell level
  - Identify spell with DC 15 + spell level

### Other Changes and Clarifications

- Potions require a bonus action to drink, not an action
- You cannot use both your action and your bonus action to cast spells of level
  1 or higher in the same turn.

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

# TODOs

- Consider if sorcerer changes are overtuned given availability of feats (ease
  of taking Metamagic Adept)
- Consider boosted healing rules (spells/potions heal max or double dice if
  healing creature above 0 HP)
