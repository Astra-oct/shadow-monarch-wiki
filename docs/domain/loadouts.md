# ⚔️ Onglet LOADOUTS

L'onglet **LOADOUTS** vous permet de créer des compositions d'armée prédéfinies pour différentes situations tactiques.

---

## 🎯 Concept

### Qu'est-ce qu'un Loadout ?

**Un Loadout est :**

- 📋 Une **liste prédéfinie** d'Ombres
- 👥 Organisée en **Squads** (groupes tactiques)
- 🎯 **Activable** d'un clic
- ⚔️ **Invoquée** via Monarch's Army

**Exemple :**
```
Loadout "Boss Raid"
├─ Squad "Vanguard" (5 Ravagers)
├─ Squad "DPS" (10 Shadow Knights)
└─ Squad "Support" (10 Skeletons)
Total : 25 Ombres, 35 slots
```

---

### Pourquoi Utiliser des Loadouts ?

**Avantages :**

✅ **Switch rapide** entre compositions  
✅ **Organisation tactique** (squads)  
✅ **Économie cognitive** (préparé à l'avance)  
✅ **Optimisation mana** (compositions ciblées)

**Sans Loadout :**
```
Invoquer Army → Toutes les Ombres (100) → 1100 mana
```

**Avec Loadout :**
```
Invoquer "Exploration" → 10 Ombres → 200 mana
Invoquer "Boss Raid" → 30 Ombres → 400 mana
```

---

## 🖥️ Interface

### Vue d'Ensemble

```
┌─────────────────────────────────────────────────┐
│  LOADOUTS - 3/5 Saved                           │
├─────────────────────────────────────────────────┤
│  [+ Create New Loadout]                         │
│                                                 │
│  ● Boss Raid               (35 slots, 25 Ombres)│
│     3 Squads | Active                           │
│     [Edit] [Duplicate] [Delete]                 │
│  ─────────────────────────────────────────────  │
│  ○ Exploration             (10 slots, 10 Ombres)│
│     1 Squad                                     │
│     [Edit] [Duplicate] [Delete] [Activate]      │
│  ─────────────────────────────────────────────  │
│  ○ PvP War                 (80 slots, 70 Ombres)│
│     5 Squads                                    │
│     [Edit] [Duplicate] [Delete] [Activate]      │
│                                                 │
│  ─────────────────────────────────────────────  │
│  Empty Slots: 2/5                               │
└─────────────────────────────────────────────────┘
```

---

## ➕ Créer un Loadout

### Étape 1 : Nouveau Loadout

**Clic sur [+ Create New Loadout] :**

```
┌──────────────────────────────────────┐
│  Create New Loadout                  │
├──────────────────────────────────────┤
│  Name: [Boss Raid_______] ✏️         │
│                                      │
│  Description (optional):             │
│  [For difficult bosses___]          │
│  [_____________________]             │
│                                      │
│  Template (optional):                │
│  ○ Empty                             │
│  ○ Copy from existing                │
│  ○ Quick Setup (Auto-fill)           │
│                                      │
│     [Cancel]        [Create]         │
└──────────────────────────────────────┘
```

---

### Option : Name

**Champ texte :**
- Max 20 caractères
- Lettres, chiffres, espaces, underscore
- Exemples : "Boss Raid", "Farm XP", "Defense_Base"

---

### Option : Template

#### ○ Empty
**Loadout vide** → Vous ajoutez manuellement les Ombres

#### ○ Copy from existing
```
Copy from: [▼ Exploration]
```
**Duplique** un Loadout existant comme base

#### ○ Quick Setup
```
Auto-fill with:
○ All Tier 1 (mass)
○ Balanced mix (T1-T3)
○ Elite only (T3-T4-T5)
```
**Remplit automatiquement** selon template

---

### Étape 2 : Ajouter des Ombres

**Après création, interface d'édition s'ouvre :**

```
┌─────────────────────────────────────────────────┐
│  Edit Loadout: Boss Raid                        │
├────────────────┬────────────────────────────────┤
│  Army (42)     │  Current Loadout (0/100 slots)│
│                │                                │
│ 🔍 [search]    │  [Empty - Drag shadows here]   │
│                │                                │
│ [T1] Zombie_01 │                                │
│ [T1] Skel_01   │                                │
│ [T2] Creep_01  │                                │
│ [T3] Ravager_1 │                                │
│ [T4] Beru      │                                │
│ [T5] Dragon    │                                │
│      ...       │                                │
│                │                                │
│                │  Squads: [Create Squad]        │
│                │                                │
├────────────────┴────────────────────────────────┤
│  Slots: 0/100  |  Mana Cost: 100  |  [Save]    │
└─────────────────────────────────────────────────┘
```

---

### Méthode 1 : Drag & Drop

**Procédure :**
1. **Gauche (Army)** : Cliquer sur une Ombre
2. **Drag** (glisser) vers droite
3. **Drop** dans "Current Loadout"
4. ✅ Ombre ajoutée !

**Visuel :**
```
Avant :
Current Loadout (0/100 slots)
[Empty]

Après drop de Beru :
Current Loadout (2/100 slots)
[⚔️ Beru] (T4, 2 slots)
```

---

### Méthode 2 : Double-Clic

**Procédure :**
1. **Double-clic** sur Ombre (gauche)
2. ✅ Ajoutée automatiquement à droite

**Plus rapide que drag & drop.**

---

### Méthode 3 : Sélection Multiple

**Procédure :**
1. **Shift+Clic** plusieurs Ombres (gauche)
2. **Clic droit** sur sélection
3. Menu : **[Add to Loadout]**
4. ✅ Toutes ajoutées

**Utile pour ajouter 10+ Ombres rapidement.**

---

### Retirer des Ombres

**Procédure :**
1. **Clic droit** sur Ombre (droite)
2. Menu : **[Remove from Loadout]**
3. ✅ Retirée (retourne à gauche)

**Alternative :** Drag depuis droite vers gauche

---

## 👥 Système de Squads

### Qu'est-ce qu'un Squad ?

**Un Squad = Groupe tactique d'Ombres**

**Caractéristiques :**
- 📊 **Formation coordonnée** (Line, Triangle, Circle)
- 🧠 **AI groupée** (restent ensemble)
- ⚙️ **Comportement unifié** (tous Aggressive, etc.)
- 🎯 **Commandes futures** (focus target, etc.)

**Max 5 Squads par Loadout**

---

### Créer un Squad

**Clic sur [Create Squad] :**

```
┌──────────────────────────────────────┐
│  Create Squad                        │
├──────────────────────────────────────┤
│  Name: [Vanguard_______] ✏️          │
│                                      │
│  Assign Shadows:                     │
│  (Select from Current Loadout)       │
│                                      │
│  [x] Ravager_1                       │
│  [x] Ravager_2                       │
│  [x] Ravager_3                       │
│  [ ] Beru                            │
│  [ ] Dragon                          │
│       ...                            │
│                                      │
│     [Cancel]        [Create]         │
└──────────────────────────────────────┘
```

---

### Configuration Squad

**Après création :**

```
┌──────────────────────────────────────┐
│  Squad: Vanguard (3 members)        │
├──────────────────────────────────────┤
│  Behavior:                           │
│    ● Aggressive                      │
│    ○ Defensive                       │
│    ○ Passive                         │
│    ○ Hold Position                   │
│                                      │
│  Formation:                          │
│    ○ Line                            │
│    ● Triangle                        │
│    ○ Circle                          │
│    ○ Scattered                       │
│                                      │
│  Position in Army:                   │
│    ○ Front (Tank role)               │
│    ● Middle (Balanced)               │
│    ○ Back (Support/Ranged)           │
│                                      │
│  [Preview Formation]  [Save]         │
└──────────────────────────────────────┘
```

---

### Option : Behavior (Squad)

**S'applique à TOUTES les Ombres du Squad :**

| Mode | Usage |
|------|-------|
| **Aggressive** | Charge ennemis, focus kill |
| **Defensive** | Protège joueur, reste proche |
| **Passive** | Suit uniquement, n'attaque pas |
| **Hold Position** | Garde un point fixe |

---

### Option : Formation

#### ○ Line (Ligne)

**Visuel :**
```
🛡️ 🛡️ 🛡️ 🛡️ 🛡️
```

**Usage :** Bloquer passage, wall

---

#### ● Triangle (Défaut)

**Visuel :**
```
    🛡️
   ⚔️ ⚔️
  🏹 🏹 🏹
```

**Usage :** Tanks devant, DPS milieu, support derrière

---

#### ○ Circle (Cercle)

**Visuel :**
```
   ⚔️  ⚔️
 ⚔️  🎯  ⚔️
   ⚔️  ⚔️
```

**Usage :** Entourer cible (boss, joueur à protéger)

---

#### ○ Scattered (Dispersé)

**Visuel :**
```
⚔️     ⚔️
   ⚔️
      ⚔️  ⚔️
```

**Usage :** Éviter AOE, harcèlement

---

### Option : Position in Army

**Détermine le positionnement relatif au joueur :**

| Position | Distance | Rôle |
|----------|----------|------|
| **Front** | 5-10 blocs devant | Tanks, charge |
| **Middle** | 2-5 blocs autour | Balanced, protection |
| **Back** | 5-10 blocs derrière | Ranged, support |

---

### Exemple de Loadout avec Squads

**Loadout "Boss Raid" :**

```
Squad 1 : "Vanguard" (Formation Triangle, Front)
├─ 5 Ravagers (Tier 3)
└─ Behavior: Aggressive

Squad 2 : "Elite Strike" (Formation Line, Middle)
├─ 10 Shadow Knights (Tier 4)
└─ Behavior: Aggressive

Squad 3 : "Ranged Support" (Formation Scattered, Back)
├─ 10 Skeletons (Tier 1)
└─ Behavior: Defensive

Total : 25 Ombres, 35 slots
Mana : 100 + (10×25) = 350
```

---

## 🎯 Activer un Loadout

### Loadout Actif

**Seul le Loadout avec ● peut être invoqué.**

**Pour activer :**
1. Cliquer **[Activate]** à côté du Loadout
2. ● Apparaît (ancien désactivé)
3. 💬 Message : *"Loadout 'Boss Raid' activated"*

**Le Loadout actif est invoqué quand vous castez "Monarch's Army".**

---

## 📊 Statistiques Loadout

### Panneau Info (Bas)

```
┌─────────────────────────────────────┐
│  Loadout: Boss Raid                 │
│                                     │
│  Shadows: 25                        │
│  Slots: 35/100                      │
│  Squads: 3                          │
│                                     │
│  Invoke Cost: 350 mana              │
│  Recall Cost: 50 mana               │
│                                     │
│  Estimated DPS: 1,250/s             │
│  Combined HP: 8,500                 │
│  Combined DEF: 1,200                │
└─────────────────────────────────────┘
```

**Calculé en temps réel** selon Ombres sélectionnées.

---

## 🔄 Éditer un Loadout

### Ouvrir Éditeur

**Clic sur [Edit] :**

**Interface identique à création**, mais pré-remplie.

**Modifications possibles :**
- ➕ Ajouter Ombres
- ➖ Retirer Ombres
- 👥 Modifier Squads
- 📝 Renommer Loadout

**Cliquer [Save] pour appliquer.**

---

## 📋 Dupliquer un Loadout

### Fonction

**Créer une copie** d'un Loadout existant.

**Usage :**
- Créer variantes (ex: "Boss Raid v2")
- Tester compositions sans perdre l'original
- Base pour nouveau Loadout

**Procédure :**
1. Clic **[Duplicate]**
2. Nouveau nom : "Boss Raid (Copy)"
3. ✅ Loadout dupliqué
4. Éditer la copie

---

## ❌ Supprimer un Loadout

### Confirmation

**Clic sur [Delete] :**

```
┌──────────────────────────────────────┐
│  Delete Loadout: Boss Raid           │
├──────────────────────────────────────┤
│  This action is permanent.           │
│  Shadows will NOT be deleted         │
│  (they return to Army).              │
│                                      │
│     [Cancel]        [Confirm]        │
└──────────────────────────────────────┘
```

**Après confirmation :**
- ✅ Loadout supprimé
- ✅ Ombres retournent dans Army (intactes)
- ✅ Slot Loadout libéré (4/5 → 3/5)

---

## 💡 Exemples de Loadouts

### "Exploration" (Early Game)

```
Composition :
- 5 Zombies (tanks légers)
- 5 Skeletons (DPS ranged)

Total : 10 Ombres, 10 slots
Mana : 200

Usage : Exploration safe, peu de mana
```

---

### "Farm XP" (Mid Game)

```
Squad "Mass" :
- 30 Tier 1 (mix Zombies/Skeletons/Spiders)

Total : 30 Ombres, 30 slots
Mana : 400

Usage : Clear rapide mobs, farm XP/loot
```

---

### "Boss Raid" (Late Game)

```
Squad 1 "Tanks" :
- 10 Ravagers (Formation Line, Front)

Squad 2 "DPS" :
- 10 Shadow Knights (Formation Triangle, Middle)

Squad 3 "Support" :
- 10 Skeletons (Formation Scattered, Back)

Total : 30 Ombres, 40 slots
Mana : 400

Usage : Boss difficiles, raids
```

---

### "Apocalypse" (Endgame)

```
Squad 1 "Titans" :
- 1 Ender Dragon
- 1 Wither
- 1 Warden

Squad 2 "Elite" :
- 10 Shadow Knights (Full Netherite)

Squad 3 "Mass" :
- 50 Tier 1-2

Total : 63 Ombres, 100 slots (FULL)
Mana : 730

Usage : Détruire TOUT
```

---

## ⚙️ Options Avancées

### Auto-Organize

**Bouton dans éditeur :**

```
[Auto-Organize Squads]
```

**Fonction :**
- Analyse vos Ombres
- Crée automatiquement 3 Squads :
  - Squad "Tanks" (tous Tier 3)
  - Squad "DPS" (tous Tier 2 + T4)
  - Squad "Support" (tous Tier 1 ranged)

**Gain de temps si composition complexe.**

---

### Import/Export

**Partager Loadouts avec amis :**

```
[Export Loadout]
→ Code généré : "BOSS-RAID-X7F9..."
→ Copier/Envoyer

[Import Loadout]
→ Coller code
→ Loadout recréé (si Ombres disponibles)
```

**Utile pour serveurs, communautés.**

---

## 🔊 Sons & Feedback

### Sons d'Action

| Action | Son |
|--------|-----|
| **Créer Loadout** | *Chime* succès |
| **Ajouter Ombre** | *Pop* doux |
| **Activer Loadout** | *Whoosh* puissant |
| **Delete** | *Fade out* |

---

## ❓ FAQ

### "Mon Loadout dépasse 100 slots"

**Message :**
```
⚠️ Loadout exceeds capacity (105/100)
```

**Solution :**
1. Retirer 5 slots d'Ombres
2. OU remplacer Tier 3 par Tier 1 (moins de slots)
3. Sauvegarder quand ≤ 100

---

### "Je ne peux pas activer un Loadout"

**Causes possibles :**
- Loadout vide (0 Ombres)
- Loadout corrompu (rare)

**Solution :**
1. Éditer → Vérifier Ombres
2. Ajouter au moins 1 Ombre
3. Réessayer

---

### "Squads ne restent pas groupés en combat"

**Causes possibles :**
- AI individuelle prime sur squad (par design)
- Ombres tombées (despawn)
- Distances trop grandes

**Amélioration future :** Commandes squad directes (en dev).

---

## 🎓 Prochaines Étapes

!!! success "Optimiser Vos Tactiques"
    - [Stratégies de Builds →](../strategies/builds.md)
    - [Combos Sorts + Loadouts →](../strategies/combos.md)
    - [PvP avec Loadouts →](../strategies/pvp.md)

---

!!! quote "Conseil"
    *"Plusieurs Loadouts bien conçus valent mieux qu'un seul massif. Adaptez-vous."*