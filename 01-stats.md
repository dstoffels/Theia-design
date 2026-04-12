Any edits made in this subtree on the [main game repository](https://github.com/dstoffels/Theia.git) must be pushed to the [Theia-design](https://github.com/dstoffels/Theia-design.git) repository:
```bash
git subtree push --prefix=design https://github.com/dstoffels/Theia-design.git main
```

# Stats

## Attributes
There are 8 attributes that serve as the core for a character's Skills & Vitals. Attribute levels are assigned at character creation and modified by the character's Lineage. As you level up your skills, skill points (SP) are allocated to the skill's associated attributes, leveling them up with every 100SP.

### Vitality
Physical fitness, endurance, and resistance to harm or environmental extremes.

### Strength
Raw physical power, reflecting the ability to exert force, break barriers, and endure heavy physical strain.

### Agility
Swift and graceful movement, representing balance, speed and reflexes. It defines the fluidity of motion in physical activity.

### Dexterity
Fine motor skills, representing precision, steadiness, and control. It encompasses tasks requiring finesse and skillful handling.

### Discipline
Focus, self-control, and mental fortitude. It signifies the ability to stay composed and consistent under pressure.

### Intellect
Abstract reasoning, comprehension, and problem-solving. It reflects the capacity for logic, learning, and mastery of knowledge.

### Presence
Passion, creativity, and influence over other beings, representing the depth of spiritual connection. 

### Acuity
Keenness of the senses, reflecting a character’s awareness, intuition, and ability to respond quickly to their surroundings.

---
## Vitals
Vitals are the current state of your character's physical and mental faculties. While each is slightly different, they all share the following properties:

Level: The vital's current state.
Max: The highest possible level for the vital, derived from associated attribute levels.
Min: The lowest possible level for the vital, the inverse of max or 0.
Impairment: The current level of impairment imparted by the vital on any abilities performed.
Tolerance: The point at which impairment begins if the vital's level drops below or goes above.
Recovery Rate: The amount of points a vital recovers per pulse (there are 30 pulses per second).

### Stamina
The amount of energy you have to spend on abilities that require physical exertion.

**Attribute Weights**
- Vitality: 2
- Strength: 1
- Agility: 1
- Dexterity: 1

### Focus
The amount of energy you have to spend on abilities that require brainpower.

**Attribute Weights**
- Discipline: 2
- Intellect: 1
- Presence: 1
- Acuity: 1

### Health
A character's current physical condition, derived directly from Vitality. Death occurs when its level reaches 0. Damaged Body Parts bleed out and reduce the recovery rate of Health. Poisons and illness can also reduce maximum health and recovery rate.

**Attribute Weights**
- Vitality: 4
- Strength: 2

### Psyche
A character's current mental and spiritual condition, derived directly from Discipline. It represents the ability to withstand psychological and spiritual trauma. Death occurs when its level reaches 0. Psyche is affected by curses, toxins and psionic attacks.

**Attribute Weights**
- Discipline: 4
- Presence: 2

### Temperature
A thermal equilibrium between hot and cold that can be affected by the environment or spells. When a character's temperature drops below the minimum tolerance, agility is reduced, slowing them down. Too hot, and the character's stamina and focus recovery is reversed.

**Attribute Weights**
- Vitality: 2
- Discipline: 2

---

## Anatomies
A humanoid anatomy is comprised of 13 **bodyparts**, generally grouped by 6 **armor slots**. Each bodypart has its own hitpoints (HP), representing the amount of damage it can withstand before becoming **impaired** or **crippled**. The max HP is derived from the average of vitality and strength.

A bodypart is impaired when its HP drop below half its maximum (damage threshold). Impaired bodyparts no longer recover HP, require medical treatment and impart a penalty on its associated attributes equal to the damage threshold - current HP level.

A bodypart is crippled when its HP reaches 0. HP can drop below 0, requiring more healing to bring it out of the crippled state. Crippled bodyparts cannot be used for combat or actions that require them, along with any of their connected **appendages**. **Critical** bodyparts kill the player when crippled. If a body part is crippled, its appendages are also crippled, but this does not affect the HP of the appendages. 

A bodypart's **size** determines its chance or difficulty of being hit during combat. Chance to hit is determined by the size of the target bodypart relative to the total size of all bodyparts. 

| Bodypart   | Critical | Size | Appendages                   | Attributes                        |
|------------|----------|------|------------------------------|-----------------------------------|
| Head       | X        | 2    |                              | Discipline, Intellect, Presence, Acuity |
| Face       | X        | 1    |                              | Presence, Acuity                  |
| Neck       | X        | 1    |                              | Discipline, Presence              |
| Chest      | X        | 4    | Abdomen, Left Arm, Right Arm | Discipline                        |
| Abdomen    |          | 4    | Left Leg, Right Leg          | Agility                           |
| Left Arm   |          | 4    | Left Hand                    | Dexterity                         |
| Left Hand  |          | 2    |                              | Dexterity                         |
| Right Arm  |          | 4    | Right Hand                   | Dexterity                         |
| Right Hand |          | 2    |                              | Dexterity                         |
| Left Leg   |          | 5    | Left Foot                    | Agility                           |
| Left Foot  |          | 3    |                              | Agility                           |
| Right Leg  |          | 5    | Right Foot                   | Agility                           |
| Right Foot |          | 3    |                              | Agility                           |
