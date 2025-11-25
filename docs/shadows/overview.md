# 👥 Système d'Ombres - Vue d'Ensemble

Les **Ombres** sont le cœur du mod Shadow Monarch. Ce sont des créatures fidèles créées à partir de monstres vaincus qui combattent éternellement à vos côtés.

---

## 🎯 Qu'est-ce qu'une Ombre ?

### Définition

Une **Ombre** est une entité invoquée qui :

- 👤 **Copie** un mob vaincu (apparence + capacités)
- 💙 **Obéit** au joueur qui l'a créée
- ⚔️ **Combat** les ennemis automatiquement
- ♾️ **Ne meurt jamais** définitivement (respawn)
- 📦 **Se stocke** dans votre Army (100 slots max)

---

## 🎨 Apparence Visuelle

### Caractéristiques Distinctives

**Toutes les Ombres partagent :**

1. 👁️ **Yeux bleus brillants** (signature visuelle)
2. 🎨 **Texture assombrie** (grise/noire)
3. ✨ **Particules noires** qui s'échappent du corps
4. 💨 **Trail sombre** en mouvement
5. 🌫️ **Aura subtile** violette/noire

!!! info "Reconnaissable Instantanément"
    Les yeux bleus permettent de distinguer vos Ombres des mobs hostiles classiques.

---

### Comparaison Visuelle

| Mob Original | Ombre |
|--------------|-------|
| Zombie (vert) | Zombie Ombre (gris foncé) |
| Skeleton (blanc) | Skeleton Ombre (noir) |
| Creeper (vert) | Creeper Ombre (gris) |
| Enderman (noir) | Enderman Ombre (noir + yeux bleus) |
| Dragon (noir) | Dragon Ombre (noir + aura violette) |

---

## 📊 Les 5 Tiers d'Ombres

### Hiérarchie

```
Tier 1 : Soldats       (1 slot)  - Masse
Tier 2 : Élites        (1 slot)  - DPS/Spécial
Tier 3 : Commandants   (1 slot)  - Tanks
Tier 4 : Shadow Knights (2 slots) - Équipables
Tier 5 : Boss          (10 slots) - Ultime puissance
```

### Vue d'Ensemble Rapide

| Tier | Type | Slots | Nombre Max | Exemples |
|------|------|-------|------------|----------|
| **1** | Soldats | 1 | ∞ | Zombie, Skeleton, Spider |
| **2** | Élites | 1 | ∞ | Creeper, Enderman, Vindicator |
| **3** | Commandants | 1 | ∞ | Ravager, Piglin Brute, Evoker |
| **4** | Shadow Knights | 2 | 20 | Joueurs morts (PvP) |
| **5** | Boss | 10 | 1/type | Dragon, Wither, Warden |

!!! info "Capacité Totale"
    **100 slots maximum** d'Army. Gérez intelligemment votre espace !

---

## 🔢 Système de Slots

### Pourquoi des Slots ?

**Balance du gameplay :**
- Empêche d'avoir 1000 Ombres (lag + OP)
- Force des choix tactiques
- Valorise les Ombres puissantes

---

### Calcul d'un Loadout

**Exemple de composition :**

```
10 Tier 1 (Zombies)      = 10 slots
5 Tier 2 (Creepers)      = 5 slots
3 Tier 3 (Ravagers)      = 3 slots
2 Tier 4 (Shadow Knights)= 4 slots
1 Tier 5 (Dragon)        = 10 slots
                         ________
                Total    = 32 slots (sur 100)
```

---

### Loadout Maximum Théorique

**Quelle est l'armée la plus puissante possible ?**

```
1 Ender Dragon    = 10 slots
1 Wither          = 10 slots
1 Warden          = 10 slots
10 Shadow Knights = 20 slots (2×10)
50 Tier 1-2-3     = 50 slots
                  _________
                Total = 100 slots
```

!!! success "Build Ultime"
    3 Boss + 10 Knights + 50 Soldats/Élites = Domination absolue

---

## 📈 Stats des Ombres

### Scaling Basé sur le Joueur

**Principe :** Les stats des Ombres sont des **pourcentages** de vos propres stats.

**Exemple :**
```
Vous avez :
- 100 HP
- 20 ATK
- 15 DEF
- 0.3 SPD

Votre Zombie Ombre (Tier 1) aura :
- 80 HP   (80% × 100)
- 12 ATK  (60% × 20)
- 13.5 DEF (90% × 15)
- 0.21 SPD (70% × 0.3)
```

---

### Coefficients par Tier

| Tier | HP | ATK | DEF | SPD |
|------|-----|-----|-----|-----|
| **Tier 1** | 70-90% | 50-70% | 80-100% | 70-90% |
| **Tier 2** | 60-80% | 100-150% | 30-50% | 100-120% |
| **Tier 3** | 150-200% | 80-100% | 120-150% | 60-80% |
| **Tier 4** | 150% | 120% + équip | 100% + équip | 110% |
| **Tier 5** | 400-500% | 130-150% | 200-250% | 110-120% |

!!! info "Évolution Automatique"
    Quand VOUS devenez plus fort (armure, enchantements), vos Ombres aussi !

---

### Croissance Exponentielle

**Exemple progressif :**

| Phase | Vos Stats | Zombie Ombre HP | Dragon Ombre HP |
|-------|-----------|-----------------|-----------------|
| **Early** | 100 HP | 80 | - |
| **Mid** | 200 HP | 160 | - |
| **Late** | 400 HP | 320 | 2000 |
| **Endgame** | 600 HP | 480 | 3000 |

**Plus vous progressez, plus vos Ombres deviennent redoutables.**

---

## ⚔️ Comportement des Ombres

### 3 Modes Disponibles

#### 🛡️ Defensive (Par Défaut)

**Comportement :**
- Suit le joueur (10 blocs max)
- Attaque si ennemis < 16 blocs
- Défend le joueur si attaqué
- Reste proche

**Usage :** Exploration, protection

---

#### ⚔️ Aggressive

**Comportement :**
- Cherche activement les ennemis
- Charge dès détection (32 blocs)
- Ne reste pas proche du joueur
- Focus kill

**Usage :** Farm, clear zones

---

#### 🕊️ Passive

**Comportement :**
- Suit uniquement
- N'attaque JAMAIS (même si frappé)
- Juste cosmétique

**Usage :** Déplacement pacifique, villages

---

#### 🚫 Hold Position

**Comportement :**
- Reste en place (ne suit pas)
- Attaque ennemis proches
- Garde un point

**Usage :** Défense de base, checkpoints

---

### Configuration

**Comment changer le comportement :**

1. Entrer dans Monarch's Domain
2. GUI → Onglet ARMY
3. Sélectionner une Ombre
4. ⚙️ Settings → Behavior
5. Choisir : Defensive / Aggressive / Passive / Hold

---

## 💀 Mort des Ombres

### Que se passe-t-il à 0 HP ?

**Les Ombres ne meurent PAS définitivement !**

**Séquence :**
1. HP atteint 0
2. 💨 **Ombre se dissout** (particules noires)
3. 💬 Message : *"[Nom] has fallen."*
4. 📦 **Reste dans votre Army** (stockée)
5. ✅ **Réinvocable** à 100% HP

!!! success "Armée Éternelle"
    Une fois une Ombre créée, elle vous appartient pour toujours. Aucune perte permanente.

---

### Réanimer une Ombre

**Procédure :**

```
1. Rappeler l'armée (Monarch's Army)
2. Attendre 30s (cooldown)
3. Réinvoquer l'armée
→ L'Ombre tombée revient à 100% HP !
```

**Coût :** 50 mana (rappel) + coût invocation

---

## 🚫 Règles Importantes

### Pas de Destruction de Terrain

**TOUTES les Ombres sont non-grief :**

| Ombre | Capacité Originale | Ombre Version |
|-------|-------------------|---------------|
| **Creeper** | Explosion casse blocs | Explosion 0 blocs détruits |
| **Wither** | Skulls détruisent terrain | Skulls 0 blocs cassés |
| **Enderman** | Ramasse/place blocs | Ne touche AUCUN bloc |
| **Ravager** | Casse blocs en chargeant | Charge sans dégâts terrain |

!!! success "Safe pour Votre Base"
    Vous pouvez invoquer 100 Ombres dans votre base sans risque de destruction !

---

### Impossibilité de Farm

**Les Ombres ne peuvent PAS :**

- ❌ Miner des blocs
- ❌ Collecter des items
- ❌ Ouvrir des coffres
- ❌ Activer des leviers/boutons
- ❌ Interagir avec le monde

**Elles sont UNIQUEMENT des combattantes.**

---

### Target Prioritaire

**Ordre d'attaque des Ombres :**

1. 🎯 **Ennemis attaquant le joueur** (priorité absolue)
2. ⚔️ **Ennemis attaquant une autre Ombre**
3. 👁️ **Mobs hostiles proches** (selon comportement)
4. 🚫 **Ignorent mobs passifs** (vaches, cochons, etc.)

---

## 📦 Stockage & Persistance

### Système d'Army

**Toutes vos Ombres sont stockées dans votre "Army" :**

- 💾 **Sauvegarde automatique** (même en déconnexion)
- 🌍 **Persistante** entre dimensions
- 📊 **Capacité : 100 slots**
- 🔍 **Accessible via Monarch's Domain GUI**

---

### Que se passe-t-il si... ?

**Vous vous déconnectez :**
- ✅ Ombres invoquées despawn
- ✅ Restent dans l'Army
- ✅ Réinvocables à la reconnexion

**Vous mourez :**
- ❌ Ombres invoquées despawn immédiatement
- ✅ Restent dans l'Army
- ✅ Réinvocables après respawn
- ⚠️ **SAUF avec Monarch Armor Set Bonus** : Ombres persistent 60s

**Vous changez de dimension :**
- ❌ Ombres ne suivent PAS (despawn)
- ✅ Restent dans l'Army
- ✅ Réinvocables dans la nouvelle dimension

---

## 🎮 Loadouts & Squads

### Système de Loadout

**Un Loadout = Une composition prédéfinie d'Ombres**

**Caractéristiques :**
- 📋 **5 Loadouts max** sauvegardables
- 👥 **5 Squads max** par Loadout
- 🎯 **1 Loadout actif** à la fois
- 🔄 **Changeable** dans Monarch's Domain

---

### Système de Squad

**Un Squad = Un groupe tactique d'Ombres**

**Avantages :**
- 📊 **Formation coordonnée** (Line/Triangle/Circle)
- 🧠 **AI améliorée** (reste groupé)
- ⚙️ **Comportement unifié** (tous Aggressive, etc.)
- 🎯 **Commandes de groupe** (futur feature)

---

### Exemple de Loadout

**Loadout "Boss Raid" :**

```
Squad 1 - "Vanguard" (Formation Triangle)
├─ 3 Ravagers (Tier 3) - Tanks devant
├─ 2 Shadow Knights (Tier 4) - DPS milieu
└─ 5 Skeletons (Tier 1) - Archers derrière

Squad 2 - "Heavy Support"
├─ 1 Wither (Tier 5) - AOE
└─ 5 Creepers (Tier 2) - Explosifs

Total : 16 Ombres, 31 slots utilisés
```

---

## 🔍 Registry JSON

### mob_tiers.json

**Seuls les mobs listés dans ce fichier peuvent être Arise.**

**Structure :**
```json
{
  "tier1": [
    "minecraft:zombie",
    "minecraft:skeleton",
    "minecraft:spider",
    "minecraft:cave_spider"
  ],
  "tier2": [
    "minecraft:creeper",
    "minecraft:enderman",
    "minecraft:vindicator",
    "minecraft:pillager"
  ],
  "tier3": [
    "minecraft:ravager",
    "minecraft:piglin_brute",
    "minecraft:evoker"
  ],
  "tier4": [
    "player"
  ],
  "tier5": [
    "minecraft:ender_dragon",
    "minecraft:wither",
    "minecraft:warden"
  ]
}
```

---

### Ajouter des Mobs Moddés

**Si vous avez un mod avec des créatures custom :**

1. Ouvrir `mob_tiers.json`
2. Ajouter le mob dans le tier approprié
3. Format : `"mod_id:mob_name"`

**Exemple (Alex's Mobs) :**
```json
{
  "tier2": [
    "minecraft:creeper",
    "alexsmobs:grizzly_bear"
  ]
}
```

!!! warning "Serveur/Modpack"
    Modification du JSON nécessite redémarrage du serveur.

---

## 💡 Stratégies de Base

### Early Game (1-20 Ombres)

**Focus :**
- Tier 1 majoritaire (facile à obtenir)
- Mix Zombies (tank) + Skeletons (DPS)
- 1-2 Creepers si Arise niveau 3+

---

### Mid Game (20-50 Ombres)

**Focus :**
- Diversification Tier 1-2-3
- Premiers Ravagers (tanks lourds)
- Organisation en Loadouts

---

### Late Game (50-100 Ombres)

**Focus :**
- Shadow Knights (PvP ou PvE)
- Boss Ombres (Dragon, Wither, Warden)
- Build optimisé avec Squads tactiques

---

## 📊 Statistiques Intéressantes

**Avec 100 slots :**

- **Max Tier 1 :** 100 Ombres
- **Max Tier 5 :** 10 Boss (théorique, mais limité à 3 types)
- **Max Shadow Knights :** 50 (mais limité à 20)

**Build équilibré typique :**
- 30 Tier 1 (masse)
- 20 Tier 2 (DPS)
- 15 Tier 3 (tanks)
- 10 Shadow Knights (élite)
- 3 Boss (ultime)
= **78 Ombres, 98 slots**

---

## 🎓 Prochaines Étapes

!!! success "Approfondir"
    - [Les 5 Tiers en Détail →](tiers.md)
    - [Mécaniques Avancées →](mechanics.md)
    - [Shadow Knights →](shadow-knights.md)

---

!!! quote "Philosophie"
    *"Une Ombre seule est faible. Une armée d'Ombres est invincible."*