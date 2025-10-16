---

## GAME DESIGN DOCUMENT: "Creature Farm Breeding Sim"

**Last Updated:** 2025-10-16
**Status:** In Development
**Version:** 0.3

---

# TABLE OF CONTENTS

1. [Core Vision & Pillars](#1-core-vision--pillars)
2. [Target Audience & Market](#2-target-audience--market)
3. [Core Gameplay Loop](#3-core-gameplay-loop)
4. [Creature System](#4-creature-system)
5. [Breeding System](#5-breeding-system)
6. [Farming System](#6-farming-system)
7. [Resource & Economy System](#7-resource--economy-system)
8. [Progression & Unlocks](#8-progression--unlocks)
9. [Social Features](#9-social-features)
10. [Monetization](#10-monetization)
11. [Technical Specifications](#11-technical-specifications)
12. [Decision Log](#12-decision-log)
13. [Open Questions](#13-open-questions)

---

# 1. CORE VISION & PILLARS

## Vision Statement
A cozy, whimsical creature breeding and farming game where players build their own fantasy farm ecosystem. Players can specialize as breeders, farmers, or hybrids, with meaningful social interdependence through collaborative breeding and resource trading.

## Target Vibe
- Cute and whimsical (like Adopt Me!, Grow a Garden)
- Relaxing/chill (minimal pressure, no timers)
- Fantasy setting with player-customized habitats
- Community-focused (requires other players)

## Core Pillars

| Pillar | Description | Why It Matters |
|--------|-------------|----------------|
| **Cute & Accessible** | All creatures are adorable, no scary elements | Appeals to 8-16 year olds + cozy game fans |
| **Specialization** | Players choose to breed, farm, or hybrid | Creates playstyle diversity, replayability |
| **Social Dependency** | Breeding requires partnership with others | Organic community formation, retention |
| **Discovery** | Endless genetic combinations | Long-term engagement, exploration mentality |
| **Low Pressure** | No mandatory daily tasks, chill vibes | Mental health + accessibility |
| **Economy-Driven** | Farming/breeding create emergent gameplay | Player agency, trading, prestige |

---

# 2. TARGET AUDIENCE & MARKET

## Primary Audience
- **Age:** 8-16 years old
- **Secondary:** Adults who enjoy cozy games (18-35)
- **Platforms:** Roblox (primary)
- **Device:** Mobile + PC

## Psychographic Profile
- Enjoys collection games (Pokémon, Adopt Me!)
- Likes relaxation/chill experiences
- Values social interaction & trading
- Interested in genetics/breeding mechanics
- Appreciates creativity (decorating, customizing)

## Competitive Analysis

| Game | Similarity | Difference |
|------|-----------|-----------|
| **Adopt Me!** | Collection, social, cute pets | Add farming + breeding strategy |
| **Grow a Garden** | Farming, relaxing, habitats | Add creatures, breeding, social |
| **Pokémon** | Breeding, collecting, trading | Simpler, cozier, less battle-focused |
| **Neopets** | Economy, creatures, trading | More modern, mobile-first, social |

---

# 3. CORE GAMEPLAY LOOP

## Daily Session (15-45 min depending on playstyle)

### Morning (5-10 min)
1. Log in, see creatures
2. Pet/interact with creatures (happiness boost)
3. Check farming progress
4. Water/fertilize 1-2 creatures (optional active farming)
5. Harvest ready crops
6. Check breeding requests from friends

### Midday (Optional)
1. More active farming if available
2. Accept/negotiate breeding trades
3. Check market listings
4. Trade resources with friends

### Evening (5-10 min)
1. Final harvest before sleep
2. Start new farming cycles
3. Plan next breeding strategy
4. Decorate habitat (optional)

## Weekly Session (30-60 min)
1. Breeding offspring arrival
2. Evaluate new genetics
3. Plan next breeding partnership
4. Trade on market
5. Participate in events (if any)

## Monthly Session (Long-term)
1. Evaluate breeding bloodlines
2. Retire creatures (if at limit)
3. Review prestige score
4. Set next genetic goals
5. Earn/spend cosmetics

---

# 4. CREATURE SYSTEM

## Base Creature Lineup (5 Species)

### Creature 1: FLUFFKIN
| Attribute | Details |
|-----------|---------|
| **Appearance** | Round, fluffy, big eyes, puffball with legs |
| **Vibe** | Adorable, innocent, huggable |
| **Traits** | Softness, roundness, big expressive eyes, gentle colors |
| **Base Colors** | White, cream, soft pink, light blue |
| **Special Features** | Fluffy tail, tiny horns, rosy cheeks |
| **Personality Animation** | Hops, nuzzles player, sits cutely |
| **Farming Focus** | Cloud Fluff harvester |
| **Farming Stat** | Comfort Expertise |

### Creature 2: SPARKWING
| Attribute | Details |
|-----------|---------|
| **Appearance** | Delicate, fairy-like, translucent wings, magical butterfly |
| **Vibe** | Magical, whimsical, ethereal, light |
| **Traits** | Wings, sparkles/glow, delicate, iridescent colors |
| **Base Colors** | Purple, pink, mint green, soft yellow |
| **Special Features** | Glowing antennae, shimmering wings, particle trails |
| **Personality Animation** | Flutters, leaves sparkles, hovers |
| **Farming Focus** | Essence Shard harvester |
| **Farming Stat** | Essence Attunement |

### Creature 3: PEBBLEHORN
| Attribute | Details |
|-----------|---------|
| **Appearance** | Chubby quadruped, small horns, goat-sheep hybrid |
| **Vibe** | Grounded, friendly, earthy, sturdy |
| **Traits** | Stockiness, horns, spots/markings, warm tones |
| **Base Colors** | Brown, cream, gray, rust orange |
| **Special Features** | Small curved horns, cloven hooves, wool-like texture |
| **Personality Animation** | Climbs, bleats, headbutts affectionately |
| **Farming Focus** | Stone & Hay harvester |
| **Farming Stat** | Excavation |

### Creature 4: SWIRLPOOL
| Attribute | Details |
|-----------|---------|
| **Appearance** | Serpentine, undulating body, happy face, water snake |
| **Vibe** | Playful, flowy, gentle, curious |
| **Traits** | Long body, flowing movement, wave patterns, blues/teals |
| **Base Colors** | Light blue, teal, seafoam, pale purple |
| **Special Features** | Fin-like appendages, rippling patterns, bubble particles |
| **Personality Animation** | Slithers, coils, creates water splashes |
| **Farming Focus** | Water Essence & Pearl harvester |
| **Farming Stat** | Hydro Sensitivity |

### Creature 5: LUMIMOTH
| Attribute | Details |
|-----------|---------|
| **Appearance** | Small rounded elephant-like, glowing core, wise little friend |
| **Vibe** | Magical, wise, calm, mysterious |
| **Traits** | Glow effects, trunk-like feature, jewel tones |
| **Base Colors** | Deep purple, midnight blue, emerald green, gold |
| **Special Features** | Glowing spots/runes, small trunk, crystalline texture |
| **Personality Animation** | Sits contemplatively, glow pulses, reaches trunk |
| **Farming Focus** | Gem Fragment & Void Crystal harvester |
| **Farming Stat** | Void Meditation |

## Creature Rarity System

### Rarity Tiers & How They're Determined

| Rarity | How Obtained | Gen | Traits | Breeding Limit |
|--------|-------------|-----|--------|----------------|
| **Common** | Starting creatures, basic catches | Gen 0 | Base appearance, basic stats | **6 uses** |
| **Uncommon** | Gen 1 hybrids (base + base) | Gen 1 | Blended traits, some color variation | **5 uses** |
| **Rare** | Gen 2 hybrids (hybrid + hybrid) | Gen 2 | Complex coloring, higher stats | **4 uses** |
| **Epic** | Gen 3+ complex bloodlines | Gen 3+ | Exceptional colors, perfect stat combinations | **4 uses** |
| **Legendary** | Perfect stat + color combination | Gen 2+ | Ultra-rare appearance, near-perfect stats | **3 uses** |
| **Mythic** | Multi-generational perfection | Gen 3+ | Impossible colors, flawless stats, unique glow | **3 uses** |

### Why Rarity Inverted (Commons Breed More, Rares Less)

**Reasoning:** Commons breed 6x → natural population controls scarcity of rares. Rare creatures breed 3x → precious, must use wisely. Creates natural market equilibrium.

**Economic Effect:**
- Commons flood market → cheap → utility focus
- Rares stay scarce → expensive → prestige focus
- No infinite arms race to better genetics

## Creature Stats

Each creature has these stat categories (0-100 scale):

### Base Stats (All Creatures)
- **Cuteness** - Visual appeal, breeding desirability
- **Health** - How long creature lives (no death, but affects breeding readiness)
- **Happiness** - Affects breeding readiness, engagement
- **Energy** - How much they can farm per day

### Farming Stats (Depends on Species)
- **Fluffkin:** Comfort Expertise
- **Sparkwing:** Essence Attunement, Luck
- **Pebblehorn:** Excavation, Strength
- **Swirlpool:** Hydro Sensitivity, Agility
- **Lumimoth:** Void Meditation, Wisdom

### Stat Inheritance (Genetic System)
- Base stats inherited from parents (70-90% pass rate)
- High stat + high stat = very high offspring
- High + Low = medium (random each time)
- Stats have natural variance (±5 points)
- Modifiers (rare drops) can boost +10 points permanently

### Example Stat Generation
```
Parent A: Cuteness 75
Parent B: Cuteness 60

Offspring probability:
- 40% inherit Parent A: ~73 (75 ±2)
- 40% inherit Parent B: ~58 (60 ±2)
- 20% blend: ~67 (average ±5)

Result: Offspring cuteness likely 58-73
```

---

# 5. BREEDING SYSTEM

## Breeding Mechanics

### Requirements for Breeding
1. **Both creatures must be ready:**
   - All needs met (fed, happy, healthy)
   - Correct resources accumulated (based on creature type)
   - Not on cooldown from last breeding
   - Correct stat thresholds met (min 40/100 in relevant stat)

2. **Both players must accept:**
   - Initiating player sends breeding request
   - Receiving player can accept, counter-offer, or decline
   - Agreement reached on payment (Gold)

3. **Breeding cooldown:**
   - 24 hours per creature before next breeding
   - Creatures take 6-12 hours to "recover" (can view but not breed)

### Breeding Process Flow

```
Step 1: Player A browses creatures (filter by species/rarity/stats)
Step 2: Player A finds Player B's Sparkwing
Step 3: Player A sends request: "Breed my Fluffkin with your Sparkwing for 300 Gold?"
Step 4: Player B can:
        - Accept (offspring goes to A, B gets 300 Gold)
        - Counter: "500 Gold" (A decides)
        - Decline
Step 5: Both agree → breeding happens
Step 6: Offspring appears in Player A's inventory
Step 7: Platform takes 5% fee (15 Gold) → Treasury
Step 8: Both creatures enter 24-hour cooldown
Step 9: Both creatures -1 from breeding limit
```

### Offspring Determination

**Distribution Model:** Offspring goes to initiating player (Player A)
- Predictable (players know what they're getting)
- Encourages trading (to acquire other player's offspring)
- Creates market for bred creatures

**Offspring Rarity:** 
- Gen 0 + Gen 0 → Gen 1 (Uncommon)
- Gen 1 + Gen 1 → Gen 2 (Rare)
- Gen 2+ + Gen 2+ → Gen 3+ (Epic/Legendary/Mythic)
- Rarity improves with generation if breeding carefully

**Color Inheritance:**
- 50% chance Parent A color
- 50% chance Parent B color
- 30% chance blend/new color
- Ultra-rare "perfect" combos (1 in 100+)

### Breeding Payment System

**Why Player-to-Player:**
- Creates economic activity
- Compensates creature owner for rarity
- Negotiation adds engagement
- Creates trading chains

**Price Discovery:**
```
Market determines price based on:
- Rarity of creature being borrowed
- Rarity of offspring expected
- Species combo desirability
- Breeding limit remaining

Typical Prices:
- Common + Common: 50-100 Gold
- Common + Rare: 200-400 Gold
- Rare + Rare: 400-800 Gold
- Rare + Legendary: 600-1200 Gold
- Legendary + Legendary: 1000-2000 Gold
```

**Platform Cut:**
- 5% taken by platform
- Goes to Treasury (used for events, economy management)
- Legitimate revenue generation

### Breeding Limit System (INVERTED)

| Rarity | Breeding Uses | Strategy |
|--------|---------------|----------|
| **Common** | 6 uses | Breed freely, hunt perfect genes |
| **Uncommon** | 5 uses | Experiment, learning phase |
| **Rare** | 4 uses | Use when confident in pairing |
| **Epic** | 4 uses | Valuable, breed with purpose |
| **Legendary** | 3 uses | Precious, save for perfect match |
| **Mythic** | 3 uses | Ultra-rare, single legendary offspring |

**Display:**
```
Creature Status: "Blossom" (Fluffkin, Rare)
Breeding Limit: 2/4 remaining
Breeding Cooldown: Ready in 3 hours

Visual indicator: Green → Yellow → Red as limit approaches
```

---

# 6. FARMING SYSTEM

## Farming Overview

**Philosophy:** Farming is a resource generation engine. Required to breed, enables specialization.

**Models Supported:**
- Pure farming (5 farming creatures)
- Pure breeding (buy/trade all resources)
- Hybrid (2-3 farmers, 2-3 breeders)
- Specialist (focus on rare drops)

## Farming Cycle

### Base Cycle (Completely Passive)
```
Day 1, 8:00 AM: Plant crop → 2 hour timer
Day 1, 10:00 AM: Harvest automatically (even if offline)
Day 1, 10:01 AM: Crop regrows → 2 hour timer
(repeats indefinitely)
```

**Base Yield (No Active Engagement):**
```
Pebblehorn Stone farm: 10 Stone per harvest
Sparkwing Essence farm: 5 Essence Shards per harvest
Swirlpool Water farm: 8 Water Essence per harvest
Fluffkin Cloud farm: 10 Cloud Fluff per harvest
Lumimoth Gem farm: 3 Gem Fragments per harvest
```

### Active Engagement (Optional, Increases Rewards)

Players can actively ten
