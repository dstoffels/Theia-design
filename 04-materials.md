Any edits made in this subtree on the [main game repository](https://github.com/dstoffels/Theia.git) must be pushed to the [Theia-design](https://github.com/dstoffels/Theia-design.git) repository:
```bash
git subtree push --prefix=design https://github.com/dstoffels/Theia-design.git main
```

# Materials
**Raw materials** are extracted from **resource nodes**, and then processed into **refined materials** and **components** at specialized stations. **Recipes** of raw, refined and component materials are used to craft other materials, items and structures. Recipes can have a **main ingredient**, which is a class of materials containing stats that combine with equipment to yield the final stats of an equipment item when crafting.

## Resources
Resources nodes contain raw materials that can be extracted with hand tools or structures. When harvesting raw materials, the player can choose which materials yielded by the node to keep or ignore. Ignored materials will pile up on the ground. This process can be automated so the character can fill its inventory and return to a settlement to store the mats and repeat until the node is depleted.

### Mineral Deposits
Some mineral nodes are surface deposits while others run deep. Deep deposits must first be manaually depleted on the surface and then a structure can be built to extract from the high-yield underground deposists. Certain nodes cannot be deep deposits and can only be mined from the surface. 

#### Clay Pit
A muddy surface deposit of clay, which is a key ingredient in construction. Clay pits can be found everywhere and are easy to extract.

**Skill**: Masonry
Action: Dig
Difficulty: 50

**Surface Yields**
| Material | Low | High  |
| --- | --- | --- |
| Clay | 100 | 300 |

---

#### Obsidian Flow
A surface deposit found near volcanic regions made of obsidian, a volcanic glass used in crafting equipment. 

**Skill**: Masonry
Action: Pry
Difficulty: 50

**Surface Yields**
| Material | Low | High  | 
| --- | --- | --- | 
| Obsidian | 50 | 150 | 

---

#### Fumarole
A fissure in the ground that emits steam and volcanic gases, found near volcanic regions. A fumarole is pried with a chisel to yield brimstone and trace amounts of hematite. Fumaroles are hazardous to mine, occasionally erupting with hot, toxic gases.

**Skill**: Masonry

**Surface Deposits**
Action: Pry
Difficulty: 75

**Yields**
| Material | Low | High  |
| --- | --- | --- |
| Brimstone | 50 | 200 |
| Hematite | 10 | 30 |

---

#### Outcrop
Bedrock jutting up through the surface, yielding stone, flint and sand, key ingredients in construction and smelting.

**Skill**: Masonry

**Surface Deposits**
Action: Mine
Difficulty: 100

**Yields**
| Material | Low | High | 
| --- | --- | --- |
| Stone | 100 | 300 |
| Sand | 100 | 300 |
| Flint | 100 | 300 |


**Deep Deposits**
Structure: Quarry

**Yields**
| Material | Low | High |
| --- | --- | --- |
| Stone | 1000 | 3000 |
| Sand | 1000 | 3000 |
| Flint | 1000 | 3000 |

---

#### Cassiterite Deposit
A concentration of cassiterite gravel, a tin ore that's sparse but easy to extract.

**Skill**: Masonry

**Surface Deposits**
Action: Dig
Difficulty: 50

**Yields**
| Material | Low | High |
| --- | --- | --- |
| Cassiterite | 100 | 300 |

---

#### Chalcopyrite Vein
A green-yellow vein embedded in rock, yielding small amounts of pure copper and brimstone, but mostly chalcopyrite, a copper ore.

**Skill**: Masonry

**Surface Deposits**
Action: Mine
Difficulty: 100

**Yields**
| Material | Low | High |
| --- | --- | --- |
| Chalcopyrite | 100 | 300 |
| Copper | 10 | 30 |
| Brimstone | 10 | 30 |

**Deep Deposits**
Structure: Draft Mine

**Yields**
| Material | Low | High |
| --- | --- | --- |
| Chalcopyrite | 1000 | 3000 |
| Copper | 100 | 300 |
| Brimstone | 100 | 300 |

---

#### Galena Vein
A silvery blue vein embedded in rock, yielding small amounts of Galena, a lead-silver ore. 

**Skill**: Masonry

**Surface Deposits**
Action: Mine
Difficulty: 150

**Yields**
| Material | Low | High |
| --- | --- | --- |
| Galena | 50 | 150 |
| Silver | 10 | 30 |

**Deep Deposits**
Structure: Draft Mine

**Yields**
| Material | Low | High |
| --- | --- | --- |
| Galena | 1000 | 3000 |
| Silver | 100 | 300 |

---

#### Quartz Vein
A light brown-grey vein embedded in a rockface, containing a concentrated variety of minerals and is the only source of gold outside of foraging. Surface deposits are low-yield and deep deposits are extremely rare.

**Skill**: Masonry

**Surface Deposits**
Action: Mine
Difficulty: 200

**Yields**
| Material | Low | High |
| --- | --- | --- |
| Hematite | 10 | 30 |
| Brimstone | 5 | 20 |
| Galena | 2 | 6 |
| Gold | 1 | 3 |

**Deep Deposits**
Structure: Shaft Mine

**Yields**
| Material | Low | High |
| --- | --- | --- |
| Hematite | 1000 | 3000 |
| Brimstone | 500 | 1000 |
| Galena | 200 | 600 |
| Gold | 10 | 30 |

#### Hematite Vein
A reddish-brown vein embedded in rock, yielding small amounts of Hematite, an iron ore.

**Skill**: Masonry

**Surface Deposits**
Action: Mine
Difficulty: 150

**Yields**
| Material | Low | High |
| --- | --- | --- |
| Hematite | 100 | 300 |

**Deep Deposits**
Structure: Shaft Mine

**Yields**
| Material | Low | High |
| --- | --- | --- |
| Hematite | 1000 | 3000 |

---

#### Hasperite Vein
A shimmering blue-white vein embedded in rock, yielding small amounts of Hasperite, a mithril ore. Hasperite veins are exceedingly rare, the surface deposits are very low yield.

**Skill**: Masonry

**Surface Deposits**
Action: Mine
Difficulty: 500

**Yields**
| Material | Low | High |
| --- | --- | --- |
| Hasperite | 8 | 20 |

**Deep Deposits**
Structure: Shaft Mine

**Yields**
| Material | Low | High |
| --- | --- | --- |
| Hasperite | 100 | 300 |

---

### Trees
Tree nodes primarily yield wood and wood byproducts, most of which require felling before harvesting. These trees have hitpoints that must be depleted to fell. Groves can be constructed in settlements to cultivate trees as a renewable resource.

#### Tree Trunk
Trunk nodes are what a felled tree becomes after all its yields have been extracted. It can be hewn in place with an adze (very slow) or dragged to a sawmill by a draft animal to produce lumber.

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Lumber | 500 | 1000 | Hew | Woodworking | Large wooden planks for construction. |
| Wood | 500 | 1000 | Hew | Woodworking | General crafting and construction material. |
| Woodchips | 20 | 50 | Hew | Woodworking | An ingredient in a wide variety of crafting recipes |

---

#### Tree
Large, generic trees of varying species that yield wood products. After felling and extracting all the wood, its trunk remains. Trees can be found in the wild and cultivated in groves using its seeds.

**Hitpoints**: 500 - 1000

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Wood | 100 | 300 | Chop | Woodworking | General crafting and construction material. |
| Woodchips | 10 | 30 | Chop | Woodworking | An ingredient in a wide variety of crafting recipes. |
| Tree Seeds | 10 |  | Harvest | Survival | Used to cultivate new trees and make oils. |
| Resin | 1 | 1 | Harvest | Survival | A sticky substance used to make adhesives. |

---

#### Yew Tree
An evergreen tree prized for its strength, elasticity and natural resistance to decay. Easy to chop down and often used to craft simple bows.

**Hitpoints**: 500 - 800

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Yew | 100 | 300 | Chop | Woodworking | Strong, flexible wood used for crafting bows and wands. |
| Woodchips | 10 | 30 | Chop | Woodworking | An ingredient in a wide variety of crafting recipes. |
| Yew Seeds | 10 |  | Harvest | Survival | Used to cultivate new Yew trees and make oils. |
| Resin | 1 | 1 | Harvest | Survival | A sticky substance used to make adhesives. |

---

#### Bamboo Cluster
A cluster of tall, fast-growing bamboo stalks. Bamboo produces a strong and versatile, hollow wood good for bows and blowguns, and is easy to cultivate. Unlike large trees, bamboo clusters can be harvested without felling.

**Hitpoints**: 200 - 300

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Bamboo | 100 | 300 | Chop | Woodworking | Hollow wooden chutes used for crafting bows and blowguns. |
| Bamboo Seeds | 10 |  | Harvest | Survival | Used to cultivate new bamboo clusters and make oils. |

---

#### Bodark Tree
A large, deciduous tree known as "Bow Wood", Bodark is extremely hard and heavy, making it one of the best woods for crafting bows, but is difficult to harvest and work with. After felling and extracting all the wood, a tree trunk remains. Bodark trees are rare, only found in certain areas.

**Hitpoints**: 2000 - 3000

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Bodark | 100 | 300 | Chop | Woodworking | Hard, heavy wood used for crafting bows and artifacts. |
| Woodchips | 10 | 30 | Chop | Woodworking | An ingredient in a wide variety of crafting recipes. |
| Resin | 1 | 1 | Harvest | Survival | A sticky substance used to make adhesives. |
| Bodark Seeds | 10 |  | Harvest | Survival | Used to cultivate new Bodark trees and make oils. |

---

#### Wyrwood Tree
Massive, ancient, seismonastic trees, gnarled and twisted and rarest of all. Wyrwoods use their roots to ensnare and crush anything moving near them and heal rapidly from damage. They are incredibly difficult to harvest, but yield a small amount of unique, magical wood equally as difficult to craft with. Bows, wands and staves made from Wyrwood are second to none. Wyrwood trees cannot be felled, and once harvested, the tree enters a dormant, impenetrable state for a long unknown length of time. This impenetrable state is passed to the harvested wood, which can only be worked using magical means, and is unbreakable when used in equipment.

**Hitpoints**: 5000 - 10000

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Wyrwood | 10 | 30 | Chop | Woodworking | A rare, magical wood used for crafting the best bows and artifacts. |

---

#### Mulberry Tree
A source of small amounts of silk rather than wood, Mulberry trees are small fruit-bearing trees that are the primary food source for silkworms. The fruits and seeds can be harvested for food, reagents and planting.

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Silk Filaments | 10 | 50 | Harvest | Survival | Fine threads produced by silkworms feeding on mulberry leaves. |
| Mulberries | 10 | 50 | Harvest | Survival | Edible fruits used for food and reagents. |

---

### Plants
Plants are a renewable resource that's used in textiles and oils. Wild sources have smaller yields, but the seeds can be used in gardens and plantations as a constant, renewable source of the plant's yields. 

#### Flax
A fibrous plant used for making linen and other textiles. Flax is a common plant that can be foraged from the wild or cultivated in gardens and plantations.

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Flax Fibers | 10 | 50 | Harvest | Survival | Used for making linen textiles |
| Linseed | 10 | 30 | Harvest | Survival | Used for planting, alchemy and making oils |

---

#### Cannabis
A versatile plant used for making textiles and oils. Cannabis is a common plant that can be foraged from the wild or cultivated in gardens and plantations.

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Hemp Fibers | 10 | 50 | Harvest | Survival | Used for making hemp textiles |
| Hempseed | 10 | 30 | Harvest | Survival | Used for planting, alchemy and making oils |

---

#### Gossypium
A soft, fluffy plant used for making quality textiles. Gossypium is a common plant that can be foraged from the wild or cultivated in gardens and plantations.

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Cotton Bolls | 10 | 50 | Harvest | Survival | Used for making cotton textiles |
| Cottonseed | 10 | 30 | Harvest | Survival | Used for planting and making oils |

---

#### Avaram
A large shrub with a wide range of medicinal and alchemical uses. Avaram is a common plant that can be foraged from the wild or cultivated in gardens and plantations.

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Avaram Leaves | 10 | 50 | Harvest | Survival | Used for medicinal and alchemical preparations. |
| Avaram Seeds | 10 | 30 | Harvest | Survival | Used for planting and making oils. |

---

#### Rhus
A poisonous shrub that produces berries used for alchemical ingredients, primarily for making Urushi lacquer. Rhus is a common plant that can be foraged from the wild or cultivated in gardens and plantations.

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Rhus Berries | 10 | 50 | Harvest | Survival | Used for making Urushi lacquer and toxins. |

---

#### Emmer
A versatile wheat used for food, livestock and as an ingredient for many processes and potions. Emmer is a common plant that can be foraged from the wild or cultivated in gardens and plantations.

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Grain | 100 | 300 | Harvest | Survival | Used for food, livestock feed, and as an ingredient. |
| Emmer Seeds | 10 | 30 | Harvest | Survival | Used for planting and making oils. |

---

### Animals
Animals are living nodes that can be a source of food and a wide range of materials. They can be hunted in the wild or domesticated for a renewable source of their yields, but require a constant supply of food and shelter. They can also be used as draft animals to pull carts and plows, but require training and equipment. Wild animals must be killed before they can be dressed for their yields and are wont to put up a fight.

#### Karakul
A breed of sheep with a thick coat of fleece.

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Fleece | 10 | 20 | Dress | Survival | Used for making wool textiles. |
| Flesh | 20 | 40 | Dress | Survival | Used to produce food and animal byproducts. |
| Bone | 5 | 10 | Dress | Survival | Used for crafting equipment, adhesives and medicinal ointments. |

---

#### Swine
A large, wild hog that can be hunted for its meat and hide, or domesticated as a renewable source of its yields. Swine are aggressive and difficult to domesticate.

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Small Hide | 1 | 1 | Dress | Survival | Used in leather production. |
| Flesh | 40 | 60 | Dress | Survival | Used to produce food and animal byproducts. |
| Bone | 10 | 20 | Dress | Survival | Used for crafting equipment, adhesives and medicinal ointments. |

#### Auroch
A large, wild bovine that can be hunted for its meat and hide, or domesticated as a draft animal or a renewable source of its yields. Aurochs are docile unless provoked and take a lot of time to domesticate, yielding large amounts of meat and hide.

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Flesh | 100 | 300 | Dress | Survival | Used to produce food and animal byproducts. |
| Large Hide | 1 | 1 | Dress | Survival | Used in leather production. |
| Bone | 10 | 20 | Dress | Survival | Used for crafting equipment, adhesives and medicinal ointments. |

---

#### Horse
A true beast of burden that can be domesticated for riding and labor, but requires a lot of time and resources to domesticate. Horses can be used to pull carts and plows, but require training and equipment. They can also be dressed for their hide, flesh and bone, but are more commonly used as draft animals.

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Large Hide | 1 | 1 | Dress | Survival | Used in leather production. |
| Flesh | 100 | 200 | Dress | Survival | Used to produce food and animal byproducts. |
| Bone | 10 | 20 | Dress | Survival | Used for crafting equipment, adhesives and medicinal ointments. |

---

#### Palukoo
A giant, furry, timid arachnid that's very difficult to tame. Palukoos are rare and non-poisonous, but produce a valuable silk that's very difficult to process. They are more prone to fleeing and hiding than they are to fight when provoked.

**Yields**
| Material | Low | High | Action | Skill | Description |
| --- | --- | --- | --- | --- | --- |
| Spiderdope | 10 | 30 | Harvest | Survival | A valuable silk used in high-quality textiles. |

---

## Raw Materials
Raw materials are extracted directly from resource nodes and are often refined before crafting components or finished products.

### Minerals

#### Clay
Clay is widely used in construction, found everywhere by foraging or mining surface deposits.

**Core**: No
**Unit**: kg

---

#### Stone
Stone is used in nearly all construction and can be mined with a pickaxe or quarry structure.

**Core**: No
**Unit**: kg

---

#### Sand
Sand is a byproduct of mining stone and a key ingredient in smelting and making glass.

**Core**: No
**Unit**: kg

---

#### Flint
Flint is a hard, brittle rock that's used for primitive equipment and as a firestarter.

**Core**: Yes
**Unit**: kg

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 2.6 | 100 | 0.8 | 5 | 0 |

---

#### Obsidian
Volcanic glass that breaks off into sharp, brittle chunks. Obsidian is used for crafting primitive equipment.

**Core**: Yes
**Unit**: kg

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 2.4 | 150 | 1.0 | 10 | 0 |

#### Brimstone
A yellow, sulfurous mineral used in alchemy and as a fuel source for smelting.

**Core**: No
**Unit**: g

#### Chalcopyrite
A golden-yellow ore for smelting copper, used for crafting basic tools and weapons.

**Core**: No
**Unit**: kg

#### Cassiterite
A tin ore for smelting bronze along with copper, used for crafting a variety of tools, weapons and armor.

**Core**: No
**Unit**: kg

#### Galena
A lead-silver ore for smelting silver, used for crafting currency and magical items.

**Core**: No
**Unit**: kg

---

#### Gold
Naturally occurring in its metallic form, gold is a precious metal used for crafting currency and magical items.

**Core**: Yes
**Unit**: g

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 19.3 | 50 | 1.2 | 0 | 1.1 |

---

#### Hematite
An iron ore for smelting iron, used for crafting tools, weapons, armor and construction materials.

**Core**: No
**Unit**: kg

#### Hasperite
An extremely rare, magical ore for smelting mithril, used for crafting the best equipment and artifacts.

**Core**: No
**Unit**: kg

---

### Wood

#### Wood
Branches and logs used in almost all types of crafting and construction.

**Core**: Yes
**Unit**: kg

**Stats**

| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 0.6 | 50 | 0.5 | 5 | 0 |

---

#### Bamboo
Hollow wooden stalks used for crafting bows and blowguns.

**Core**: Yes
**Unit**: kg

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 0.5 | 100 | 0.6 | 5 | 0 |

---

#### Yew
Branches from yew trees, used for crafting bows and wands.

**Core**: Yes
**Unit**: kg

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 0.7 | 200 | 0.8 | 5 | 0 |

---

#### Bodark
A distinct yellow wood from the Bodark tree, known as "Bow Wood", used for crafting excellent bows.

**Core**: Yes
**Unit**: kg

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 0.8 | 150 | 1.0 | 15 | 0 |

---

#### Wyrwood
A magical wood with unique properties, used for crafting enchanted items. Can only be worked with magical means and is unbreakable when used in equipment.

**Core**: Yes
**Unit**: kg

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 0.5 | 0 | 1.2 | 0 | 0 |


---

#### Lumber
Large wooden planks produced by hewing tree trunks, used in construction.

**Core**: No
**Unit**: kg

### Fibers

#### Flax Fibers
Fibers from the flax plant, used for making linen textiles.

**Core**: No
**Unit**: g

---

#### Hemp Fibers
Fibers from the cannabis plant, used for making hemp textiles.

**Core**: No
**Unit**: g

---

#### Cotton Bolls
Fibers from the gossypium plant, used for making cotton textiles.

**Core**: No
**Unit**: g

---

#### Silk Filaments
Fibers produced by silkworms feeding on mulberry leaves, used for making high-quality textiles.

**Core**: No
**Unit**: g

---

#### Spiderdope
A valuable silk produced by Palukoos, used for making spidersilk.

**Core**: No
**Unit**: g

---

#### Hide
A an animal hide used for making primitive armor and refining into leathers.

**Core**: Yes
**Unit**: kg

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- | --- |
| 0.9 | 100 | 0.8 | 10 | 0 |

---

### Byproducts
Miscellaneous materials that are byproducts of harvesting and processing other materials, used as ingredients in a wide variety of crafting recipes.

#### Woodchips
A byproduct of chopping wood, used as for Tannin, Vitriol and, Urushi.

**Core**: No
**Unit**: kg

---

#### Resin
A sticky substance harvested from trees, used to make adhesives.

**Core**: No
**Unit**: g

---

#### Tree Seeds
Seeds harvested from various trees, used for planting and crafting oils.

**Core**: No
**Unit**: g

---

#### Yew Seeds
Seeds from yew trees, used for planting and crafting oils.

**Core**: No
**Unit**: g

---

#### Bamboo Seeds
Seeds from bamboo plants, used for planting and crafting oils.

**Core**: No
**Unit**: g

---
#### Bodark Seeds
Seeds from Bodark trees, used for planting and crafting oils.

**Core**: No
**Unit**: g

---

#### Avaram Seeds
Seeds from the Avaram shrub, used for planting and crafting oils.

**Core**: No
**Unit**: g

---

#### Avaram Leaves
Leaves from the Avaram shrub, used for medicinal and alchemical preparations.

**Core**: No
**Unit**: g

---

#### Grain
Grains harvested from Emmer wheat, used for food, livestock feed, and as an ingredient.

**Core**: No
**Unit**: g

#### Rhus Berries
Berries from the Rhus shrub, used for planting and making Urushi lacquer and toxins.

**Core**: No
**Unit**: g

---

#### Mulberries
Fruits from the Mulberry tree, used for planting, food and reagents.

**Core**: No
**Unit**: g

---

#### Flesh
Harvested from animals to produce food and sinew.

**Core**: No
**Unit**: kg

#### Bone
A combination of bone and horn with an extensive range of uses, including crafting equipment, adhesives and medicinal ointments.

**Core**: No
**Unit**: kg

---

## Refined Materials
Materials processed at specialized stations from a recipe of raw or other refined materials. They are used to craft components, supplies, ingredients and sometimes finished products. 

### Rigids
Any hardened material from rawhide to metals. Metals are recyclable materials produced from ores, that can be smelted repeatedly with a loss ratio. Most metal items can be smelted back into ingots for repurposing, with the exception of indestructible magical metals which hold their forged shape permanently.


#### Rawhide
A stiff material made from animal hides, for making armor and shields.

**Core**: Yes
**Skill**: Husbandry
**Difficulty**: 50
**Unit**: kg

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 0.9 | 150 | 0.8 | 10 | 0 |

**Recipes**
| Material | Amount |
| --- | --- |
| Hide | 1 |
| **Station** | Tanning Rack |
| **Yield** | 1 Rawhide |

---

#### Cuirbouilli
A hard, molded leather polymer made from specially treated animal hides, used for making lightweight, yet effective heavy armor.

**Core**: Yes
**Skill**: Husbandry
**Difficulty**: 150
**Unit**: g

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 0.7 | 300 | 1.0 | 20 | 0 |

**Recipes**
| Material | Amount |
| --- | --- |
| Rawhide | 4 |
| Charcoal | 5 |
| Urushi | 1 |
| **Station** | Tanning Rack |
| **Yield** | 1 Cuirbouilli |

--- 

#### Copper
A malleable metal smelted from chalcopyrite, but also exists in a pure, native form that can be foraged and mined. Copper is the most basic metal, used for casting basic tools and weapons. Copper items cannot be repaired and must be recycled into new ingots and forged again.

**Core**: Yes
**Skill**: Metallurgy
**Difficulty**: 50
**Unit**: kg

**Recipes**
| Material | Amount |
| --- | --- |
| Chalcopyrite | 3 |
| Charcoal | 10 |
| **Station** | Kiln |
| **Yield** | 1 Copper |

**Recycling**
| Material | Amount |
| --- | --- |
| Copper | 1.5 |
| Charcoal | 10 |
| **Station** | Kiln |
| **Yield** | 1 Copper |

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 8 | 100 | 1.0 | 10 | 1 |

---

#### Bronze
A copper-tin alloy, smelted from chalcopyrite/copper and cassiterite. A significant step up from copper, but sourcing both copper and tin simultaneously can be difficult. Bronze is used for crafting a wide variety of tools, weapons and armor. Bronze items cannot be repaired and must be recycled into new ingots and forged again.

**Core**: Yes
**Skill**: Metallurgy
**Difficulty**: 100
**Unit**: kg

**Recipes**
| Material | Amount |
| --- | --- |
| Chalcopyrite | 3 |
| Cassiterite | 1 |
| Charcoal | 10 |
| **Station** | Kiln |
| **Yield** | 1 Bronze |

| Material | Amount |
| --- | --- |
| Copper | 2 |
| Cassiterite | 1 |
| Charcoal | 10 |
| **Station** | Kiln |
| **Yield** | 1 Bronze |

**Recycling**
| Material | Amount |
| --- | --- |
| Bronze | 1.5 |
| Charcoal | 10 |
| **Station** | Kiln |
| **Yield** | 1 Bronze |

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 8.8 | 1000 | 1 | 15 | 0.9 |

---

#### Silver
Smelted from Galena, silver is a very soft, precious metal that's difficult to extract from its ore. As such, Galena yields a very small amount of silver. It's used for crafting currency and magical items, but is too soft to be used for tools or weapons.

**Skill**: Metallurgy
**Difficulty**: 200
**Unit**: kg

**Recipes**
| Material | Amount |
| --- | --- |
| Galena | 10 |
| Charcoal | 5 |
| Bone | 1 |
| **Station** | Kiln |
| **Yield** | 1 Silver |

**Recycling**
| Material | Amount |
| --- | --- |
| Silver | 2 |
| Charcoal | 10 |
| **Station** | Kiln |
| **Yield** | 1 Silver |

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 10.5 | 75 | 1.1 | 0 | 1 |

---

#### Iron
A common metal smelted from hematite. Iron is equivalent to bronze, but more difficult to smelt. Iron is used for crafting tools, weapons, armor and construction materials. Iron items can easily be repaired, or recycled back into iron, giving it a distinct resource advantage over bronze.

**Skill**: Metallurgy
**Difficulty**: 200
**Unit**: kg

**Recipes**
| Material | Amount |
| --- | --- |
| Hematite | 10 |
| Charcoal | 25 |
| Sand | 2 |
| **Station** | Bloomery |
| **Yield** | 1 Iron |

**Recycling**
| Material | Amount |
| --- | --- |
| Iron | 1.5 |
| Charcoal | 25 |
| Sand | 2 |
| **Station** | Bloomery |
| **Yield** | 1 Iron |

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 7.8 | 1000 | 1 | 15 | 0.7 |

---

#### Steel
Steel is an iron-carbon alloy that's stronger and more durable than iron, used for crafting high-quality equipment. Steel items can easily be repaired, or recycled back into steel. Steel is smelted from iron rather than ore, so it has a much better yield ratio than iron.

**Skill**: Metallurgy
**Difficulty**: 300
**Unit**: kg

**Recipes**
| Material | Amount |
| --- | --- |
| Iron | 2 |
| Charcoal | 30 |
| Sand | 3 |
| Bone | 2 |
| **Station** | Bloomery |
| **Yield** | 1 Steel |

**Recycling**
| Material | Amount |
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
| 7.8 | 2000 | 1.2 | 25 | 0.6 |

---

#### Wootz
Wootz is a high-carbon crucible steel that's significantly stronger, much more durable and difficult to produce than steel. Wootz is used for crafting some the best equipment, but requires a draft furnace to smelt. Wootz is **experimental**, meaning the recipe must be discovered through player trial and error. Failed attempts will yield steel and drop hints to the player about the results. Wootz items can easily be repaired, or recycled back into wootz.

**Skill**: Metallurgy
**Difficulty**: 500
**Unit**: kg

**Recipes**
| Material | Amount |
| --- | --- |
| Iron | 2 |
| Charcoal | 51 |
| Sand | 9 |
| Avaram | 3 |
| Crucible | 1 |
| **Station** | Draft Furnace |
| **Yield** | 1 Wootz |

**Recycling**
| Material | Amount |
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
| 7.8 | 5000 | 1.4 | 30 |  0.5 |

---

#### Mithril
An extremely rare, extremely light, indestructible metal that can only be forged into a component once, requiring great skill. Smelting hasperite into mithril is an experimental process that must be discovered through player trial and error. Failed attempts will return the hasperite and drop hints to the player about the results. The smelting process requires an extremely skilled smith and an alchemist who must produce a very difficult catalyst potion from rare ingredients. While it's smelted in a draft furnace, mithril must be forged an a mana forge.

**Skill**: Metallurgy
**Difficulty**: 600
**Unit**: kg

**Recipes**
| Material | Amount |
| --- | --- |
| Hasperite | 2 |
| Charcoal | 97 |
| Sand | 14 |
| Avaram | 9 |
| Bone | 3 |
| Crucible | 1 |
| Aqua Regia | 1 |
| **Station** | Draft Furnace |
| **Yield** | 1 Mithril |

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 3.0 | 0 | 1.5 | 60 | 0 |

---

#### Rolaren
The top-tier, indestructible magical metal. A mithril alloy that can only be forged by the most skilled Smiths, Alchemists and Artificers. Rolaren is smelted from mithril using an experimental process that must be discovered through player trial and error. Failed attempts will return the mithril and drop hints to the player about the results. Rolaren must be forged an a mana forge.

**Skill**: Metallurgy
**Difficulty**: 800
**Unit**: kg

**Recipes**
| Material | Amount |
| --- | --- |
| Mithril | 2 |
| Wyrwood | 1 |
| Cassiterite | 3 |
| Avaram | 5 |
| Bone | 5 |
| Charcoal | 146 |
| Sand | 21 |
| Crucible | 1 |
| Aqua Regia | 1 |
| **Station** | Draft Furnace |
| **Yield** | 1 Rolaren |

**Stats**
| Density | Durability | DamageModifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 2.5 | 0 | 1.7 | 80 | 0 |

---

### Textiles
Textiles are refined from plant fibers and animal products in preparation for crafting rope, clothing and armor.

#### Leather
A flexible, durable material made from treated animal hides, used for making rope and padded armor.

**Core**: Yes
**Skill**: Husbandry
**Difficulty**: 100
**Unit**: g

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 0.8 | 200 | 0.9 | 15 | 0 |

**Recipes**
| Material | Amount |
| --- | --- |
| Hide | 2 |
| Tannin | 1 |
| **Station** | Tanning Rack |
| **Yield** | 1 Leather |

--- 

#### Linen
A lightweight, breathable fabric made from flax fibers, used for making clothing and bandages.

**Core**: Yes
**Skill**: Outfitting
**Difficulty**: 50
**Unit**: g

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 0.5 | 50 | 0.7 | 5 | 0 |

**Recipes**
| Material | Amount |
| --- | --- |
| Flax Fibers | 2 |
| **Station** | Spinnery |
| **Yield** | 1 Linen |

---

#### Hemp
A strong, coarse fabric made from hemp fibers, used for making rope, sacks and basic clothing.

**Core**: Yes
**Skill**: Outfitting
**Difficulty**: 50
**Unit**: g

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 0.6 | 75 | 0.8 | 10 | 0 |

**Recipes**
| Material | Amount |
| --- | --- |
| Hemp Fibers | 2 |
| **Station** | Spinnery |
| **Yield** | 1 Hemp |

---

#### Cotton
A soft, fluffy fabric made from cotton bolls, used for making clothing and armor.

**Core**: Yes
**Skill**: Outfitting
**Difficulty**: 75
**Unit**: g

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 0.5 | 50 | 0.7 | 5 | 0 |

**Recipes**
| Material | Amount |
| --- | --- |
| Cotton Bolls | 2 |
| **Station** | Spinnery |
| **Yield** | 1 Cotton |

---

#### Silk
A luxurious, lightweight and strikingly strong fabric made from silk filaments, used for making fine clothing and padded armors.

**Core**: Yes
**Skill**: Outfitting
**Difficulty**: 100
**Unit**: g

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 0.4 | 100 | 0.6 | 2 | 0 |

**Recipes**
| Material | Amount |
| --- | --- |
| Silk Filaments | 10 |
| **Station** | Spinnery |
| **Yield** | 1 Silk |

---

#### Spidersilk
An incredibly strong and elastic silken fabric made from spiderdope, used for making high-end clothing, padded armor and bowstrings.

**Core**: Yes
**Skill**: Outfitting
**Difficulty**: 200
**Unit**: g

**Stats**
| Density | Durability | Damage Modifier | Hindrance | Conductivity |
| --- | --- | --- | --- | --- |
| 0.3 | 200 | 0.5 | 1 | 0 |

**Recipes**
| Material | Amount |
| --- | --- |
| Spiderdope | 20 |
| **Station** | Spinnery |
| **Yield** | 1 Spidersilk |

---

### Supplies
Supplies are various materials spent in crafting processes or upkeep. 

#### Food
Citizen upkeep stored in settlements, 1kg consumed 3x/day for each citizen.

**Core**: No
**Skill**: Survival
**Difficulty**: 0
**Unit**: kg

**Recipes**
| Material | Amount |
| --- | --- |
| Flesh | 2 |
| Wood | 2 |
| **Station** | Campfire |
| **Yield** | 300 Sinew, 1 Food, 200 Oil |

| Material | Amount |
| --- | --- |
| Grain | 1200 |
| **Station** | Campfire |
| **Yield** | 1 Food |

---

#### Sinew
A tough, fibrous material harvested from animal flesh, used for making rope.

**Core**: No
**Skill**: Survival
**Difficulty**: 50
**Unit**: g

**Recipes**
| Material | Amount |
| --- | --- |
| Flesh | 2 |
| Wood | 2 |
| **Station** | Campfire |
| **Yield** | 300 Sinew, 1 Food, 200 Oil |

---

#### Charcoal
A carbon-rich fuel made from burning wood in a kiln.

**Core**: No
**Skill**: Survival
**Difficulty**: 50
**Unit**: kg

**Recipes**
| Material | Amount |
| --- | --- |
| Wood | 5 |
| **Station** | Kiln |
| **Yield** | 1 Charcoal |

---

#### Wire
A thin, flexible metal used for crafting intricate items and components. Wire is smelted from iron or better, and can be recycled.

**Core**: No
**Skill**: Smithing
**Difficulty**: 150
**Unit**: g

**Recipes**
| Material | Amount |
| --- | --- |
| Iron / Steel / Wootz / Mithril / Rolaren | 1 |
| Charcoal | 1 |
| **Station** | Forge |
| **Yield** | 1000 Wire |

---

### Compounds

#### Oil
A flammable liquid made from distilling seeds or flesh, used for fuel and alchemical purposes.

**Core**: No
**Skill**: Survival
**Difficulty**: 50
**Unit**: kg

**Recipes**
| Material | Amount |
| --- | --- |
| Flesh | 2 |
| Wood | 2 |
| **Station** | Campfire |
| **Yield** | 300 Sinew, 1 Food, 200 Oil |

| Material | Amount |
| --- | --- |
| [Seeds] | 100 |
| Wood | 1 |
| **Station** | Campfire |
| **Yield** | 100 Oil |

---

#### Tannin
A bitter compound made from distilling woodchips and resin, used for tanning leather.

**Core**: No
**Skill**: Alchemy
**Difficulty**: 50
**Unit**: g

**Recipes**
| Material | Amount |
| --- | --- |
| Woodchips | 5 |
| Resin | 2 |
| **Station** | Still |
| **Yield** | 100 Tannin |

---

#### Pitch
A sticky, flammable substance made from distilling resin, used as an adhesive.

**Core**: No
**Skill**: Alchemy
**Difficulty**: 50
**Unit**: g

**Recipes**
| Material | Amount |
| --- | --- |
| Resin | 5 |
| **Station** | Still |
| **Yield** | 100 Pitch |

---

#### Vitriol
A caustic compound made from distilling brimstone, charcoal and resin, used for crafting poisons.

**Core**: No
**Skill**: Alchemy
**Difficulty**: 100
**Unit**: g

**Recipes**
| Material | Amount |
| --- | --- |
| Brimstone | 200 |
| Charcoal | 3 |
| Resin | 2 |
| **Station** | Still |
| **Yield** | 100 Vitriol |

#### Urushi
A lacquer made from distilling Rhus berries, charcoal and resin, used for waterproofing and hardening leather and wood.

**Core**: No
**Skill**: Alchemy
**Difficulty**: 150
**Unit**: g

**Recipes**
| Material | Amount |
| --- | --- |
| Rhus Berries | 5 |
| Charcoal | 2 |
| Resin | 2 |
| **Station** | Still |
| **Yield** | 100 Urushi |

---




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

