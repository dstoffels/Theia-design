If edits or corrections are made in this subtree on the [main game repository](https://github.com/dstoffels/Theia.git), they must be pushed to the [Theia-design](https://github.com/dstoffels/Theia-design.git) repository:
```bash
git subtree push --prefix=design https://github.com/dstoffels/Theia-design.git main
```

# Skills

A skill is a specialized collection of abilities, equipment, techniques and spells, that earns xp whenever you invoke the skill. Your skill's level unlocks new abilities, **archetypes** and also levels up your attributes with skill points (SP). Skills are the central function of a character and its development. They dictate how you interact with the world, how your character grows and they affect all other stats, directly and indirectly.

All skills start at level 0, level up at 1000XP, with each subsequent level requiring 1% more XP than the previous. The intellect level is the amount of XP earned when a skill is invoked.

| Level |	1 |	2 |	3 |	4 |	5 |	6 |	7 |	8 |	9 |	10 |
| ----- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Level xp |	1000 |	1010 |	1020 |	1030 |	1040 |	1051 |	1062 |	1072 |	1083 |	1094 |
| Total xp |	1000 |	2010 |	3030 |	4060 |	5100 |	6151 |	7213 |	8285 |	9368 |	10462 |

Each skill is associated with two or more attributes, which are weighted (totaling 12) to determine the SP allocated to these attributes when the skill levels up. This attribute weighting also yields the skill's **Aptitude**, which combines with the skill's level to determine your **Proficiency** whenever you invoke one of its abilities, accounting for natural talent and experience.

---

## Warrior Skills
Melee combat with various infantry weapons, shields and armor. These are the most straightforward combat skills, focused on physical prowess and technique.


### Bludgeons
Maces, hammers, axes, anything with a heavy head and haft.

**Attribute Weights:**
- Strength: 6
- Vitality: 4
- Agility: 2

### Swords
Longswords, shortswords, and other long-bladed weapons.

**Attribute Weights:**
- Dexterity: 6
- Strength: 3
- Agility: 3

### Polearms
Spears, halberds, and other long-reach weapons.

**Attribute Weights:**
- Strength: 6
- Agility: 6

### Defense
Shields, armor, and other defensive combat techniques.

**Attribute Weights:**
- Strength: 6
- Vitality: 4
- Acuity: 2

---

## Rogue Skills
A combination of unconventional combat with ranged weapons, hand-to-hand and cunning, more focused on finesse, precision and guile than raw power.


### Shortblades
Short, easily concealed blades for quick strikes.

**Attribute Weights:**
- Dexterity: 6
- Agility: 6

### Archery
Bows, crossbows, and fletching.

**Attribute Weights:**
- Strength: 6
- Acuity: 4
- Dexterity: 2

### Unarmed
Hand-to-hand combat, grappling and takedowns.

**Attribute Weights:**
- Agility: 6
- Strength: 3
- Dexterity: 3

### Subterfuge
Stealth, thievery, and various thrown and projectile weapons.

**Attribute Weights:**
- Agility: 6
- Dexterity: 3
- Acuity: 3

---

## Mystic Skills
Revolving around mind and spirit, mystic skills are focused on spiritual connection, mental fortitude and the ability to influence the unseen forces of the world.


### Animism
Control of the life forces; healing and protection.

**Attribute Weights:**
- Presence: 6
- Discipline: 6

### Manifestation
Bringing the ethereal to the corporeal; summoning and reanimation.

**Attribute Weights:**
- Presence: 6
- Intellect: 6

### Psionism
Manipulation of the mind; illusions and clairvoyance.

**Attribute Weights:**
- Presence: 6
- Discipline: 4
- Acuity: 2

### Speechcraft
Sound and song to influence mind and matter.

**Attribute Weights:**
- Presence: 6
- Acuity: 3
- Discipline: 3

---

## Mage Skills
The study and manipulation of the fundamental forces of the universe. Exerting magical control over the physical world and the flow of time and space.


### Cohesion
Elemental order; crystallization and cooling.

**Attribute Weights:**
- Discipline: 8
- Intellect: 4

### Entropics
Elemental disorder; disruption and heating.

**Attribute Weights:**
- Intellect: 6
- Discipline: 3
- Acuity: 3

### Galvanics
Elemental fields; plasma and electromagnetic forces.

**Attribute Weights:**
- Intellect: 6
- Acuity: 6

### Displacement
Elemental distortion; telekinesis and spatial manipulation.

**Attribute Weights:**
- Intellect: 8
- Discipline: 4

---

## Builder Skills
The practical application of knowledge and craftsmanship to create, repair, and enhance structures, tools, and equipment.


### Woodworking
Building structures and crafting wooden components.

**Attribute Weights:**
- Dexterity: 6
- Strength: 4
- Vitality: 2

### Masonry
Mining, quarrying, and construction with stone and earth.

**Attribute Weights:**
- Vitality: 6
- Strength: 6

### Metallurgy
Smelting, forging, and crafting with metals.

**Attribute Weights:**
- Vitality: 4
- Strength: 4
- Intellect: 4

---

## Settler Skills


### Survival
Basic crafting, food preparation, and first aid.

**Attribute Weights:**
- Acuity: 8
- Vitality: 4

### Husbandry
Livestock, crop cultivation, and resource management.

**Attribute Weights:**
- Vitality: 6
- Strength: 3
- Presence: 3

### Outfitting
Clothing, cobbling, armor and textiles.

**Attribute Weights:**
- Dexterity: 6
- Acuity: 6

---

## Scholar Skills
The study and practice of alchemical and magical arts, focused on the creation of magical potions, enchantments, and artifacts.


### Alchemy
Transforming substances and creating potions.

**Attribute Weights:**
- Intellect: 7
- Acuity: 5

### Artifacts
Crafting wands, staves, talismans, and charms.

**Attribute Weights:**
- Intellect: 8
- Dexterity: 4

### Spellbinding
Embedding magical properties into objects and materials.

**Attribute Weights:**
- Intellect: 6
- Discipline: 6