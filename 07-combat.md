Any edits made in this subtree on the [main game repository](https://github.com/dstoffels/Theia.git) must be pushed to the [Theia-design](https://github.com/dstoffels/Theia-design.git) repository:
```bash
git subtree push --prefix=design https://github.com/dstoffels/Theia-design.git main
```

# Combat

Combat in Theia is all about gaining advantage by wearing down opponents' stats. 

## Damage Types
Each damage type inflicts a unique effect.

### Impact
Impact damage is the most basic type of damage. Impact always damages target equipment even if the attack is blocked or its damage is fully mitigated. Successfuly attacks cause 2x damage to armor.

### Laceration
Laceration damage inflicts a lacerated state on the target's bodypart, doubling the bleeding effect.

### Puncture
Puncture damage comes with an armor piercing effect, reducing the armor's damage mitigation. Successful attacks cause 2x damage to armor.

### Temperature
Temperature damage can be either hot or cold, which adds or reduces temperature points to the target, respectively and does not cause bleeding. Temperature damage can be used to debilitate the target, but may not directly damage them. If the bodypart is already bleeding, temp damage may stop the bleeding.

### Galvanic
Galvanic damage directly reduces the target's stamina and focus in addition to damaging the opponent. It does not cause bleeding and its effects are amplified by conductive armor. Galvanic attacks are often single strikes with long cooldowns (too OP?).

### Poison
Poison damage directly reduces the target's health and its recovery rate over time.

### Psychic
Psychic damage directly reduces the target's psyche and its recovery rate over time.

