Any edits made in this subtree on the [main game repository](https://github.com/dstoffels/Theia.git) must be pushed to the [Theia-design](https://github.com/dstoffels/Theia-design.git) repository:
```bash
git subtree push --prefix=design https://github.com/dstoffels/Theia-design.git main
```

# Materials


## Raw Materials
Raw materials are extracted directly from resource nodes and are often refined before crafting components or finished products.

### Minerals
Most minerals are dug up, mined or quarried from surface and underground deposits. Hand tools are used for extracting minerals from surface deposits, while underground deposits require a mineshaft or quarry to be built over them but yield much larger quantities. 

#### Clay
Concentrations of clay-rich soil that can be easily dug up with a shovel. Clay is used in a wide variety of construction applications. Clay is found virtually everywhere and only exists in surface deposits.

**Surface Deposit Yields (kg)**
| Material | Low | High | Action | Skill |
| --- | --- | --- | --- | --- |
| Clay | 100 | 300 | Dig | Masonry |

#### Sand
Concentrations of sand that can be easily dug up with a shovel. Sand is used in construction and as a crafting supply. Sand is found virtually everywhere and only exists in surface deposits.

**Surface Deposit Yields (kg)**
| Material | Low | High | Action | Skill |
| --- | --- | --- | --- | --- |
| Sand | 100 | 300 | Dig | Masonry |

#### Stone
Stone is found everywhere by foraging or mining surface and underground deposits. Stone is used in nearly all construction.

**Surface Deposit Yields (kg)**
| Material | Low | High | Action | Skill |
| --- | --- | --- | --- | --- |
| Stone | 100 | 300 | Mine | Masonry |

**Underground Deposit Yields (kg)**
| Material | Low | High | Structure | Skill |
| --- | --- | --- | --- | --- |
| Stone | 10000 | 30000 | Quarry | Masonry |

#### Flint
Flint is a versatile and common quartz that's found by foraging or mining surface deposits with a pickaxe. It is used for crafting primitive tools and weapons, and required for fires and a variety of construction applications.

**Surface Deposit Yields (kg)**
| Material | Low | High | Action | Skill |
| --- | --- | --- | --- | --- |
| Flint | 100 | 300 | Mine | Masonry |

#### Obsidian
Obsidian is an uncommon volcanic glass that can be mined from surface deposits with a pickaxe or foraged near volcanic areas. The sharpness of obsidian makes it ideal for crafting cutting tools and small weapons, but its brittleness makes it less durable and only suited for small items like arrowheads and spearheads.

**Surface Deposit Yields (kg)**
| Material | Low | High | Action | Skill |
| --- | --- | --- | --- | --- |
| Obsidian | 50 | 150 | Mine | Masonry |

#### Brimstone
Brimstone is an abundant, yellow crystalline mineral that can be foraged or mined near volcanic regions with a pickaxe. Brimstone is widely used in alchemy as a hot fuel source, poisons and incendiaries. 

**Surface Deposit Yields (kg)**
| Material | Low | High | Action | Skill |
| --- | --- | --- | --- | --- |
| Brimstone | 50 | 150 | Mine | Masonry |

---

#### Native Copper
Native copper is a naturally occurring form of copper metal that is only found in small amounts by foraging rather than in deposits. It's used for crafting primitive tools and weapons or can be smelted to make bronze when combined with tin.

---

#### Chalcopyrite
Chalcopyrite a common mineral that can be mined from surface deposits with a pickaxe, while underground deposits require a mineshaft. Chalcopyrite can be smelted with Cassiterite to produce bronze.

**Surface Deposit Yields (kg)**
| Material | Low | High | Action | Skill |
| --- | --- | --- | --- | --- |
| Chalcopyrite | 100 | 300 | Mine | Masonry |

#### Cassiterite
Cassiterite is a common mineral that can be mined from surface deposits with a pickaxe. Cassiterite is used to make bronze when smelted with copper or chalcopyrite.

**Surface Deposit Yields (kg)**
| Material | Low | High | Action | Skill |
| --- | --- | --- | --- | --- |
| Cassiterite | 100 | 300 | Mine | Masonry |

#### Galena
Galena is a rare silver ore that can be mined from both surface and underground deposits. Silver is often used for crafting currency and magical items.

**Surface Deposit Yields (kg)**
| Material | Low | High | Action | Skill |
| --- | --- | --- | --- | --- |
| Galena | 50 | 150 | Mine | Masonry |

**Underground Deposit Yields (kg)**
| Material | Low | High | Structure | Skill |
| --- | --- | --- | --- | --- |
| Galena | 500 | 1000 | Drift Mine | Masonry |

#### Gold Nuggets
A very rare, natural occurrence of gold that can be foraged from riverbeds and underground deposits. Gold nuggets can be smelted to make gold, commonly used to craft currency and magical items.

**Underground Deposit Yields (g)**
| Material | Low | High | Structure | Skill |
| --- | --- | --- | --- | --- |
| Gold Nuggets | 2000 | 5000 | Shaft Mine | Masonry |

#### Hematite
An iron ore that's common but much more difficult to process and only found in deposits. Hematite is used to create Iron, Steel and Wootz, but require more advanced facilities to smelt and craft with.

**Surface Deposit Yields (kg)**
| Material | Low | High | Action | Skill |
| --- | --- | --- | --- | --- |
| Hematite | 100 | 300 | Mine | Masonry |

**Underground Deposit Yields (kg)**
| Material | Low | High | Structure | Skill |
| --- | --- | --- | --- | --- |
| Hematite | 1000 | 3000 | Shaft Mine | Masonry |

#### Hasperite
Hasperite is an extremely rare, magical ore that can only be mined from deep underground in small amounts. Hasperite is a source of mithril and rolaren, two of the most prized, magical metals in the world, used for crafting the best weapons and armor.

**Underground Deposit Yields (kg)**
| Material | Low | High | Structure | Skill |
| --- | --- | --- | --- | --- |
| Hasperite | 100 | 300 | Shaft Mine | Masonry |

---

### Trees
Tree nodes primarily yield wood and other wood byproducts, most of which require felling before harvesting. These trees have hitpoints that must be depleted to fell. Groves can be constructed in settlements to cultivate trees as a renewable resource.

#### Tree
Large, generic trees of varying species that yield wood products. After felling and extracting all the wood, a trunk remains on the ground and can be hewn in place to produce lumber (very slow) or dragged to a settlement by a draft animal.

**Hitpoints**: 500 - 1000

**Yields (kg)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Wood | 100 | 300 | Chop | Woodworking | General crafting and construction material. |
| Woodchips | 10 | 30 | Chop | Woodworking | An ingredient in a wide variety of crafting recipes. |
| Trunk* | 1 | 1 | Chop | Woodworking | Can be hewn into lumber, cannot be carried. |
| Tree Seeds | 10 |  | Harvest | Survival | Used to cultivate new trees and make oils. |
| Resin | 1 | 1 | Harvest | Survival | A sticky substance used to make adhesives. |

#### Yew Tree
An evergreen tree prized for its strength, elasticity and natural resistance to decay. Easy to chop down and often used to craft simple bows.

**Hitpoints**: 500 - 800

**Yields (kg)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Yew | 100 | 300 | Chop | Woodworking | Strong, flexible wood used for crafting bows and wands. |
| Woodchips | 10 | 30 | Chop | Woodworking | An ingredient in a wide variety of crafting recipes. |
| Yew Seeds | 10 |  | Harvest | Survival | Used to cultivate new Yew trees and make oils. |
| Resin | 1 | 1 | Harvest | Survival | A sticky substance used to make adhesives. |

#### Bamboo Cluster
A cluster of tall, fast-growing bamboo stalks. Bamboo produces a strong and versatile, hollow wood good for bows and blowguns, and is easy to cultivate. Unlike large trees, bamboo clusters can be harvested without felling.

**Hitpoints**: 200 - 300

**Yields (kg)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Bamboo | 100 | 300 | Chop | Woodworking | Hollow wooden chutes used for crafting bows and blowguns. |
| Bamboo Seeds | 10 |  | Harvest | Survival | Used to cultivate new bamboo clusters and make oils. |

#### Bodark Tree
A large, deciduous tree known as "Bow Wood", Bodark is extremely hard and heavy, making it one of the best woods for crafting bows, but very difficult to harvest and work with. After felling and extracting all the wood, a trunk remains on the ground and can be hewn in place to produce lumber (very slow) or dragged to a settlement by a draft animal. Bodark trees are rare, only found in certain areas and do not yield seeds, so they cannot be cultivated.

**Hitpoints**: 2000 - 3000

**Yields (kg)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Bodark | 100 | 300 | Chop | Woodworking | Hard, heavy wood used for crafting bows and artifacts. |
| Woodchips | 10 | 30 | Chop | Woodworking | An ingredient in a wide variety of crafting recipes. |
| Trunk* | 1 | 1 | Chop | Woodworking | Can be hewn into lumber, cannot be carried. |
| Resin | 1 | 1 | Harvest | Survival | A sticky substance used to make adhesives. |

#### Wyrwood Tree
Massive, ancient, seismonastic trees, gnarled and twisted and rarest of all. Wyrwoods use their roots to ensnare and crush anything moving near them and heal rapidly from damage. They are incredibly difficult to harvest, but yield a small amount of unique, magical wood equally as difficult to craft with. Bows, wands and staves made from Wyrwood are second to none. Wyrwood trees cannot be felled, and once harvested, the tree enters a dormant, impenetrable state for a long unknown length of time. This impenetrable state is passed to the harvested wood, which can only be worked using magical means, and is unbreakable when used in equipment.

**Hitpoints**: 5000 - 10000

**Yields (kg)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Wyrwood | 10 | 30 | Chop | Woodworking | A rare, magical wood used for crafting the best bows and artifacts. |


#### Mulberry Tree
A source of small amounts of silk rather than wood, Mulberry trees are small fruit-bearing trees that are the primary food source for silkworms. The fruits and seeds can be harvested for food, reagents and planting.

**Yields (g)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Silk Filaments | 10 | 50 | Harvest | Survival | Fine threads produced by silkworms feeding on mulberry leaves. |
| Mulberry Seeds | 10 | 30 | Harvest | Survival | Used to cultivate new mulberry trees and make oils. |
| Mulberries | 10 | 50 | Harvest | Survival | Edible fruits used for food and reagents. |

---

### Plants
Plants are a renewable resource that's used in textiles and oils. Wild sources have smaller yields, but the seeds can be used in gardens and plantations as a constant, renewable source of the plant's yields. 

#### Flax Plant
A fibrous plant used for making linen and other textiles. Flax is a common plant that can be foraged from the wild or cultivated in gardens and plantations.

**Yields (g)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Flax Fibers | 10 | 50 | Harvest | Survival | Used for making linen textiles |
| Flaxseed | 10 | 30 | Harvest | Survival | Used for planting and making oils |

---

#### Cannabis
A versatile plant used for making textiles and oils. Cannabis is a common plant that can be foraged from the wild or cultivated in gardens and plantations.

**Yields (g)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Hemp Fibers | 10 | 50 | Harvest | Survival | Used for making hemp textiles |
| Hempseed | 10 | 30 | Harvest | Survival | Used for planting and making oils |

---

#### Gossypium
A soft, fluffy plant used for making quality textiles. Gossypium is a common plant that can be foraged from the wild or cultivated in gardens and plantations.

**Yields (g)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Cotton Bolls | 10 | 50 | Harvest | Survival | Used for making cotton textiles |
| Cottonseed | 10 | 30 | Harvest | Survival | Used for planting and making oils |

---

#### Avaram Senna
A large shrub with a wide range of medicinal and alchemical uses. Avaram senna is a common plant that can be foraged from the wild or cultivated in gardens and plantations.

**Yields (g)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Avaram | 10 | 50 | Harvest | Survival | Used for medicinal and alchemical preparations. |
| Avaram Seeds | 10 | 30 | Harvest | Survival | Used for planting and making oils. |

---

#### Rhus Shrub
A poisonous shrub that produces berries used for alchemical ingredients, primarily for making Urushi lacquer. 

**Yields (g)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Rhus Berries | 10 | 50 | Harvest | Survival | Used for making Urushi lacquer and toxins. |
| Rhus Seeds | 10 | 30 | Harvest | Survival | Used for planting and making oils. |

---

#### Emmer
A versatile wheat used for food, livestock and as an ingredient for many processes and potions. Emmer is a common plant that can be foraged from the wild or cultivated in gardens and plantations.

**Yields (kg)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Grain | 100 | 300 | Harvest | Survival | Used for food, livestock feed, and as an ingredient. |
| Emmer Seeds | 10 | 30 | Harvest | Survival | Used for planting and making oils. |

---

### Animals
Animals are living nodes that can be a source of food and a wide range of materials. They can be hunted in the wild or domesticated for a renewable source of their yields, but require a constant supply of food and shelter. They can also be used as draft animals to pull carts and plows, but require training and equipment. Wild animals must be killed before they can be dressed for their yields and are wont to put up a fight.

#### Karakul
A breed of sheep with a thick coat of fleece.

**Yields (kg)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Fleece | 10 | 20 | Dress | Survival | Used for making wool textiles. |
| Flesh | 20 | 40 | Dress | Survival | Used to produce food and animal byproducts. |
| Bone | 5 | 10 | Dress | Survival | Used for crafting equipment, adhesives and medicinal ointments. |

---

#### Swine
A large, wild hog that can be hunted for its meat and hide, or domesticated as a renewable source of its yields. Swine are aggressive and difficult to domesticate.

**Yields (kg)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Flesh | 40 | 60 | Dress | Survival | Used to produce food and animal byproducts. |
| Bone | 10 | 20 | Dress | Survival | Used for crafting equipment, adhesives and medicinal ointments. |

#### Auroch
A large, wild bovine that can be hunted for its meat and hide, or domesticated as a draft animal or a renewable source of its yields. Aurochs are docile unless provoked and take a lot of time to domesticate, yielding large amounts of meat and hide.

**Yields (kg)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Flesh | 100 | 300 | Dress | Survival | Used to produce food and animal byproducts. |
| Hide | 20 | 30 | Dress | Survival | Used in leather production. |
| Bone | 10 | 20 | Dress | Survival | Used for crafting equipment, adhesives and medicinal ointments. |

---

#### Horse
A true beast of burden that can be domesticated for riding and labor, but requires a lot of time and resources to domesticate. Horses can be used to pull carts and plows, but require training and equipment. They can also be dressed for their hide, flesh and bone, but are more commonly used as draft animals.

**Yields (kg)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Hide | 20 | 30 | Dress | Survival | Used in leather production. |
| Flesh | 100 | 200 | Dress | Survival | Used to produce food and animal byproducts. |
| Bone | 10 | 20 | Dress | Survival | Used for crafting equipment, adhesives and medicinal ointments. |

---

#### Pukaloo
A giant, furry, timid arachnid that's very difficult to tame. Pukaloos are rare and non-poisonous, but produce a valuable silk that's very difficult to process. They are more prone to fleeing and hiding than they are to fight when provoked.

**Yields (g)**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Spiderdope | 10 | 30 | Harvest | Alchemy | A valuable silk produced by Pukaloos, used in high-quality textiles. |

---

## Refined Materials
Refined materials are processed at specialized stations from a recipe of raw or other refined materials. They are used to craft components, supplies, ingredients and sometimes finished products. 

- Stations listed are the most basic station required to refine the material. Many stations are replaced by more advanced ones where the material can also be refined (campfire > hearth > fireplace).

### Metals
Metals are recyclable materials that can be smelted repeatedly to yield ingots of a specific mass (1 ore = 1kg metal). Even metal items can be smelted back into ingots for repurposing. Leftover mass will be returned as a smaller ingot when crafting and multiple ingots can be combined in the smelting process for larger ingots.


#### Copper
Copper is a malleable metal smelted from native copper or chalcopyrite, used for casting basic tools and weapons. As such, it's not a very durable metal, but it's easy to work with and can be smelted with tin to make bronze, which is stronger and more durable. Copper items cannot be repaired and must be recycled into new ingots and forged again.

**Skill**: Metallurgy
**Difficulty**: 50
**Unit**: 1kg

**Recipes**
| Material | Amount (kg) |
| --- | --- |
| Native Copper | 1 |
| Charcoal | 5 |
| **Station** | Kiln |
| **Yield** | 1 Copper |

| Material | Amount (kg) |
| --- | --- |
| Chalcopyrite | 3 |
| Charcoal | 10 |
| **Station** | Kiln |
| **Yield** | 1 Copper |

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 8 | 100 | 1.0 | 10 | 1 |

---

#### Bronze
Bronze is an alloy of copper and tin, smelted from chalcopyrite, native copper, copper and cassiterite. It's harder and more durable than copper, but slightly more difficult to smelt and work with. Bronze items are cast from the ingots rather than forged, so they cannot be repaired and must be recycled into new ingots and recast.

**Skill**: Metallurgy
**Difficulty**: 100
**Unit**: 1kg

**Recipes**
| Material | Amount (kg) |
| --- | --- |
| Chalcopyrite | 3 |
| Cassiterite | 1 |
| Charcoal | 10 |
| **Station** | Kiln |
| **Yield** | 1 Bronze |

| Material | Amount (kg) |
| --- | --- |
| Native Copper | 2 |
| Cassiterite | 1 |
| Charcoal | 10 |
| **Station** | Kiln |
| **Yield** | 1 Bronze |

| Material | Amount (kg) |
| --- | --- |
| Copper | 2 |
| Cassiterite | 1 |
| Charcoal | 10 |
| **Station** | Kiln |
| **Yield** | 1 Bronze |

**Recycling**
| Material | Amount (kg) |
| --- | --- |
| Bronze | 1.5 |
| Charcoal | 10 |
| **Station** | Kiln |
| **Yield** | 1 Bronze |

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 8.8 | 500 | 1 | 15 | 0.9 |

---

#### Silver
Smelted from Galena, silver is a very soft, precious metal that's difficult to extract from its ore. As such, Galena yields a very small amount of silver. It's used for crafting currency and magical items, but is too soft to be used for tools or weapons.

**Skill**: Metallurgy
**Difficulty**: 200
**Unit**: 1kg

**Recipes**
| Material | Amount (kg) |
| --- | --- |
| Galena | 10 |
| Charcoal | 5 |
| Bone | 1 |
| **Station** | Kiln |
| **Yield** | 1 Silver |

**Recycling**
| Material | Amount (kg) |
| --- | --- |
| Silver | 2 |
| Charcoal | 10 |
| **Station** | Kiln |
| **Yield** | 1 Silver |

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 10.5 | 75 | 1.1 | 0 | 1 |

#### Gold
Smelted from gold nuggets, gold is the softest metal. Gold is highly valuable and used for crafting currency and magical items, but is too soft to be used for tools or weapons. It's so rare that it's measured in grams rather than kilograms.

**Skill**: Metallurgy
**Difficulty**: 250
**Unit**: 1g

**Recipes**
| Material | Amount (g) |
| --- | --- |
| Gold Nuggets | 10 |
| Charcoal | 5 |
| **Station** | Kiln |
| **Yield** | 8 Gold |

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 19.3 | 50 | 1.2 | 0 | 1.1 |

#### Iron
Iron is a strong, durable metal used for crafting tools, weapons, armor and is also used in construction. Iron items can easily be repaired, giving them a resource advantage over copper and bronze, but they are more difficult to smelt and work with. Iron can also be used to smelt steel and wootz, which are significant upgrades over iron, but require more advanced facilities to smelt and craft with. Hematite is incredibly abundant, but only yields about 10% iron when smelted.

**Skill**: Metallurgy
**Difficulty**: 250
**Unit**: 1kg

**Recipes**
| Material | Amount (kg) |
| --- | --- |
| Hematite | 10 |
| Charcoal | 25 |
| Sand | 2 |
| **Station** | Bloomery |
| **Yield** | 1 Iron |

**Recycling**
| Material | Amount (kg) |
| --- | --- |
| Iron | 1.5 |
| Charcoal | 25 |
| Sand | 2 |
| **Station** | Bloomery |
| **Yield** | 1 Iron |

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 7.8 | 1000 | 1 | 20 | | 0.7 |

---

#### Steel
Steel is an iron-carbon alloy that's stronger and more durable than iron, but more difficult to smelt and work with. Steel is used for crafting high-quality tools, weapons and armor. Steel items can easily be repaired, or recycled back into steel. Steel is smelted from iron rather than ore, so it has a much higher yield than iron.

**Skill**: Metallurgy
**Difficulty**: 350
**Unit**: 1kg

**Recipes**
| Material | Amount (kg) |
| --- | --- |
| Iron | 2 |
| Charcoal | 30 |
| Sand | 3 |
| Bone | 2 |
| **Station** | Bloomery |
| **Yield** | 1 Steel |

**Recycling**
| Material | Amount (kg) |
| --- | --- |
| Steel | 1.2 |
| Charcoal | 30 |
| Sand | 3 |
| Bone | 2 |
| **Station** | Bloomery |
| **Yield** | 1 Steel |

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 7.8 | 2000 | 1.2 | 25 | | 0.6 |

---

#### Wootz
Wootz is a high-carbon steel alloy that's significantly stronger, much more durable and more difficult to produce than steel. Wootz is used for crafting some the best equipment, but requires a draft furnace to smelt. Wootz is experimental, meaning the recipe must be discovered through player trial and error. Failed attempts will yield steel and drop hints to the player about the results. Wootz items can easily be repaired, or recycled back into wootz. Wootz is smelted from iron rather than ore.

**Skill**: Metallurgy
**Difficulty**: 500
**Unit**: 1kg

**Recipes**
| Material | Amount (kg) |
| --- | --- |
| Iron | 5 |
| Charcoal | 51 |
| Sand | 9 |
| Avaram | 3 |
| Crucible | 1 |
| **Station** | Draft Furnace |
| **Yield** | 1 Wootz |

**Recycling**
| Material | Amount (kg) |
| --- | --- |
| Wootz | 1.1 |
| Charcoal | 51 |
| Sand | 9 |
| Avaram | 3 |
| Crucible | 1 |
| **Station** | Draft Furnace |
| **Yield** | 1 Wootz |

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 7.8 | 5000 | 1.4 | 30 | | 0.5 |

---

#### Mithril
Mithril is an extremely rare, extremely light, indestructable metal that can only be forged into a component once, requiring great skill. Smelting hasperite into mithril is an experimental process that must be discovered through player trial and error. Failed attempts will just return the hasperite and drop hints to the player about the results. The smelting process requires an extremely skilled smith and an alchemist who must produce a very difficult catalyst potion from rare ingredients. While it's smelted in a draft furnace, mithril must be forged an a mana forge.

**Skill**: Metallurgy
**Difficulty**: 600
**Unit**: 1kg

**Recipes**
| Material | Amount (kg) |
| --- | --- |
| Hasperite | 2 |
| Charcoal | 97 |
| Sand | 14 |
| Crucible | 1 |
| Catalyst Potion | 1 |
| **Station** | Draft Furnace |
| **Yield** | 1 Mithril |

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 5.0 | 0 | 1.5 | 60 | 0 |


| Ingot | Station | Materials | Level | Description |
| --- | --- | --- | --- | --- |
| Copper | Campfire | Chalcopyrite, Charcoal | 0 | A soft, malleable metal used for basic tools and weapons |
| Bronze | Kiln | Chalcopyrite, Cassiterite, Charcoal | 50 | An alloy of copper and tin, harder than copper and used for a variety of tools, weapons and armor |
| Silver | Kiln | Galena, Charcoal | 50 | A precious metal used for crafting currency and magical items |
| Gold | Kiln | Gold Nuggets, Charcoal | 50 | A highly valuable metal used for crafting currency and magical items |
| Iron | Smelter | Hematite, Charcoal | 100 | A strong, durable metal used for tools, weapons, and armor |
| Steel | Bloomery | Hematite, Charcoal | 200 | An iron-carbon alloy, strong and durable, used for high-quality equipment |
| Wootz | Draft Furnace | Experimental | 300 | A high-carbon steel alloy, significantly stronger and more difficult to produce than steel |
| Mithril | Mana Forge | Experimental | 500 | An extremely rare, indestructable metal that can only be forged once, requiring great skill |
| Rolaren | Mana Forge | Experimental | 700 | A magical mithril alloy that can only be forged by the most skilled Smiths, Alchemists and Artificers |

### Textiles
Textiles are refined from plant fibers and animal products in preparation for crafting rope, clothing and armor.

**Skills**: Accoutrements, Husbandry. Survival

| Textile | Station | Materials | Level | Description |
| --- | --- | --- | --- | --- |
| Sinew | Campfire | Flesh | 0 | A tough, fibrous material used for string or rope |
| Rawhide | Tanning Rack | Hide | 50 | A stiff, durable material used for basic armor and shields |
| Leather | Tanning Rack | Hide, Tannin | 100 | A flexible, durable material used for padded armor |
| Cuirbouilli | Tanning Rack | Hide, Tannin, Urushi | 200 | A stiff, molded leather used for quality padded armor |
| Linen | Spinnery | Flax Fibers | 50 | A lightweight, breathable fabric used for clothing and bandages |
| Hemp | Spinnery | Hemp Fibers | 50 | A strong, coarse fabric used for rope, sacks and basic clothing |
| Cotton | Spinnery | Cotton Bolls | 50 | A soft, fluffy fabric used for clothing and bedding |
| Silk | Spinnery | Silk Filaments | 100 | A luxurious, smooth fabric used for fine clothing and bedding |
| Spidersilk | Spinnery | Spiderdope,  | 200 | A strong, flexible fabric with natural elasticity and water resistance, used for high-end clothing and armor |


### Supplies
Supplies are various materials spent in crafting processes or upkeep.

**Skills**: Alchemy, Woodworking

| Supply | Station | Materials | Level | Description |
| --- | --- | --- | --- | --- |
| Charcoal | Kiln | Wood | 0 | A carbon-rich fuel used for smelting, alchemy and firing ceramics |
| Pitch | Campfire | Resin | 50 | A sticky, flammable substance used for waterproofing and adhesives |
| Food | Campfire | Wood, Flesh, Grain | 0 | Citizen upkeep stored in settlements, 1kg consumed 3x/day for each citizen |
| Oil | Campfire | Flesh, Seeds | 50 | A flammable liquid used for fuel, alchemical purposes |
| Lumber | Sawmill | Trunk | 50 | Processed wood used for advanced construction |
<!-- | Resin | Alembic | Resin | 50 | A sticky, flammable substance used for waterproofing and adhesives | -->
| Tannin | Alembic | Wood, Resin | 50 | A bitter compound used for tanning leather and dyeing textiles |
| Vitriol | Alembic | Brimstone, Charcoal, Resin | 100 | A caustic compound used for crafting poisons |
| Urushi | Alembic | Rhus Berries, Charcoal, Resin | 150 | A lacquer used for waterproofing and hardening leather and wood |
| Wire | Forge | Bronze+, Charcoal | 150 | A thin, flexible metal used for crafting intricate items and components |


---

## Components
Components are the building blocks for crafting items. Some are replaceable modules used to enhance existing items, like the pommel of a sword. Even after crafting, modules can be reclaimed by disassembling an item, allowing the player to repurpose them into entirely different items.

The materials used to make a component will impart their qualities into the crafted item. The durability of iron is greater than that of copper, but less than that of steel. For weapons, different materials affect weight or damage; for armor, its hindrance or damage reduction.

### Blades
- Thin: A narrow blade with a sharp point.
- Broad: A wide, straight blade for crafting swords.
- Curved: A short, curved blade for crafting swords.
- Convex: A wide, curved blade for crafting swords.
- Leaf: A broad, rounded, 2-sided blade for crafting shortblades.
- Tapered: A triangular 2-sided blade for crafting daggers.
- Knife: A small, 1-sided blade for crafting knives.

### Heads
| Component | Materials | Station | Description |
| --- | --- | --- | --- |
| Grip | Wood \ Bone \ Leather \ Rawhide \ Leather | Workbench | A handle for swords and shortblades, can be single, double or bastard. |
| Knife Blade | Bone \ Flint \ Obsidian \ Copper+ | Kiln+ | A small blade for crafting knives (1-edge). |
| Tapered Blade | Copper+ | Kiln+ | A triangular blade for crafting daggers (2-edge). |
| Recurved Blade | Copper+ | Kiln+ | A curved blade for crafting daggers (1-edge). |
| Thin Blade | Bronze+ | Kiln+ | A narrow blade for crafting swords & daggers (5 sizes, 2-edge). |
| Broad Blade | Bronze+ | Kiln+ | A wide, straight blade for crafting swords (3 sizes, 2-edge). |
| Curved Blade | Bronze+ | Kiln+ | A short, curved blade for crafting swords (3 sizes, 1-edge). |
| Convex Blade | Bronze+ | Kiln+ | A wide, curved blade for crafting swords (3 sizes, 1-edge). |
| Shaft | Wood | Workbench | A wooden haft for crafting polearms and bludgeons of varying lengths. |
| Spearhead | Flint \ Obsidian \ Copper+ | Kiln+ | A short, tapered blade for crafting polearms. |
| Hammerhead | Stone \ Copper+ | Kiln+ | A blunt head for crafting hammer-based bludgeons & tools (2 sizes). |
| Axehead | Stone \ Copper+ | Kiln+ | A bladed head for crafting axe-based blugeons. |
| Macehead | Stone \ Copper+ | Kiln+ | A spiked head for crafting mace-based bludgeons. |
| Adzehead | Stone \ Copper+ | Kiln+ | A bladed head with a perpendicular edge for crafting adze-based weapons/tools. |

### Armor Components
| Component | Materials | Station | Description |
| --- | --- | --- | --- |
| Kozane | Wood \ Bone \ Cuirbouilli \ Copper+ | Forge | Small, rigid plates for crafting lamellar & laminar armor (heavy). |
| Lame | Wood \ Bone \ Cuirbouilli \ Copper+ | Forge | Long, rigid strips for crafting laminar armor (heavy). |
| Plate | Copper+ | Forge | Large, rigid sheets for crafting plate armor (heavy). |







<!-- ## Raw Materials
Raw materials are extracted directly from resource nodes and are often refined before crafting components or finished products.

- Refined materials denoted with an asterisk require multiple materials to create.

### Minerals
Minerals come from **deposits** and can sometimes be gathered from the environment in small amounts by foraging (Survival). 

**Skill**: Masonry

| Material       | Refines to       | 
| -------------- | ---------------- |
| Clay           |                  |
| Sand           |                  |
| Flint          |                  |
| Stone          |                  |
| Obsidian       |                  |
| Brimstone      |                  |
| Chalcopyrite   | Copper, Bronze*  |
| Cassiterite    | Bronze*          |
| Galena      | Silver*           |
| Gold Nuggets     | Gold*             |
| Hematite       | Iron*, Steel*     |
| Hasperite      | Mithril*, Rolaren*|

### Wood
**Skill**: Woodworking

| Material | Refines to |
| --- | --- |
| Wood | Shaft, Charcoal, Tannin* |
| Trunk | Lumber |
| Yew |  |
| Bamboo |  |

### Fibers
**Skill**: Survival

| Material | Refines to |
| --- | --- |
| Flax Fibers | Linen |
| Hemp Fibers | Hemp |
| Cotton Bolls | Cotton |
| Silk Filaments | Silk |
| Hide | Rawhide, Leather*, Cuirbouilli* |


### Byproducts
Byproducts are miscellaneous materials harvested from all resources often used for food, medicines and alchemical reagents.

| Material | Refines to |
| --- | --- |
| Woodchips | Tannin*, Vitriol*, Urushi* |
| Flesh | Food, Sinew |
| Rhus Berries | Urushi* |
| Grain | Food  |
| Avaram |  |
| Mulberries |  | -->