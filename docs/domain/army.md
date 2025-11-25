# 📋 Onglet ARMY

L'onglet **ARMY** est votre registre complet de toutes les Ombres que vous possédez. C'est ici que vous gérez chaque unité individuellement.

---

## 🎯 Fonction Principale

### À quoi sert cet onglet ?

**Gestion individuelle des Ombres :**

- 📜 **Voir la liste complète** de vos Ombres
- 🔍 **Rechercher** une Ombre spécifique
- 🎚️ **Filtrer** par tier, statut, équipement
- ⚙️ **Configurer** chaque Ombre (nom, comportement)
- 🎽 **Équiper** Shadow Knights
- ❌ **Release** Ombres inutiles

---

## 🖥️ Interface

### Vue d'Ensemble

```
┌─────────────────────────────────────────────────┐
│  ARMY - 42/100 Slots                            │
├─────────────────────────────────────────────────┤
│  🔍 Search: [____________]  [x]                 │
│                                                 │
│  Filters: [All] [T1] [T2] [T3] [T4] [T5]       │
│           [Stored] [Deployed]                   │
│                                                 │
│  Sort by: [▼ Alphabetical]                      │
├─────────────────────────────────────────────────┤
│                                                 │
│  [🧟 Zombie_01]    Tier 1  |  1 slot           │
│     HP: 80  ATK: 12  DEF: 18                   │
│     Status: Stored                              │
│     [⚙️ Settings] [❌ Release]                  │
│  ─────────────────────────────────────────────  │
│  [⚔️ Beru]         Tier 4  |  2 slots          │
│     HP: 300  ATK: 56  DEF: 45                  │
│     Status: Deployed                            │
│     Equipment: Full Netherite                   │
│     [⚙️ Settings] [🎽 Equipment] [❌ Release]   │
│  ─────────────────────────────────────────────  │
│  [🐉 Dragon_01]    Tier 5  |  10 slots         │
│     HP: 1000  ATK: 225  DEF: 625               │
│     Status: Stored                              │
│     [⚙️ Settings] [❌ Release]                  │
│                                                 │
│                    [...]                        │
│                                                 │
└─────────────────────────────────────────────────┘
```

---

## 🔍 Barre de Recherche

### Utilisation

**Recherche en temps réel :**

```
🔍 Search: [zombie]

Résultats affichés :
- Zombie_01
- Zombie_02
- Zombie_Elite
```

---

### Syntaxe Avancée

**Recherche par critères :**

| Critère | Syntaxe | Exemple |
|---------|---------|---------|
| **Nom** | Texte simple | `Beru` |
| **Type** | Nom mob | `skeleton` |
| **Tier** | `T1`, `Tier 3` | `T4` |
| **HP** | `HP>100` | `HP>200` |
| **ATK** | `ATK<50` | `ATK>30` |
| **Slots** | `slots:2` | `slots:10` |

---

### Exemples de Recherche

**Trouver tous les Shadow Knights :**
```
T4
ou
Tier 4
ou
slots:2
```

**Trouver les Ombres puissantes :**
```
HP>300
```

**Trouver un mob spécifique :**
```
dragon
```

---

## 🎚️ Système de Filtres

### Filtres par Tier

**Boutons de filtre rapide :**

```
[All] [T1] [T2] [T3] [T4] [T5]
```

**Fonctionnement :**
- **Clic simple** : Affiche uniquement ce tier
- **Shift+Clic** : Ajoute ce tier à la sélection
- **All** : Réinitialise (affiche tout)

**Exemple :**
```
Clic [T1] → Affiche 30 zombies/skeletons
Shift+Clic [T2] → Affiche T1 + T2 (50 Ombres)
Clic [All] → Affiche les 100 Ombres
```

---

### Filtres par Statut

```
[Stored] [Deployed] [Equipped]
```

| Filtre | Description |
|--------|-------------|
| **Stored** | Ombres en stockage (non invoquées) |
| **Deployed** | Ombres actuellement invoquées |
| **Equipped** | Shadow Knights avec équipement |

**Combinaison possible :**
```
[T4] + [Deployed] = Shadow Knights invoqués actuellement
```

---

## 📊 Système de Tri

### Options Disponibles

**Menu déroulant :**

```
Sort by: [▼ Alphabetical]
```

**Options :**

1. **Alphabetical** (A→Z)
   - Zombie_01 → Zombie_02 → Beru → Dragon_01

2. **Tier** (1→5)
   - Tous T1 → Tous T2 → ... → Tous T5

3. **Date Added** (récent→ancien)
   - Dernière Ombre créée en haut

4. **Power** (HP × ATK décroissant)
   - Dragon_01 (225000) → Beru (16800) → Zombie_01 (960)

5. **Slots Used** (croissant)
   - Tier 1 (1 slot) → Tier 4 (2 slots) → Tier 5 (10 slots)

---

## 📝 Carte d'Ombre (Détails)

### Informations Affichées

**Chaque Ombre affiche :**

```
[🧟 Zombie_01]         ← Icône + Nom
Tier 1  |  1 slot      ← Tier + Coût slots
HP: 80  ATK: 12  DEF: 18  SPD: 0.084  ← Stats
Status: Stored         ← Statut actuel
Behavior: Defensive    ← Comportement
Created: 2h ago        ← Date d'Arise

[⚙️ Settings] [❌ Release]  ← Actions
```

---

### Icônes par Type

| Type | Icône | Couleur |
|------|-------|---------|
| **Zombie** | 🧟 | Vert |
| **Skeleton** | 💀 | Blanc |
| **Spider** | 🕷️ | Rouge |
| **Creeper** | 💣 | Vert clair |
| **Enderman** | 🌀 | Violet |
| **Ravager** | 🦏 | Gris |
| **Shadow Knight** | ⚔️ | Bleu |
| **Dragon** | 🐉 | Noir/violet |
| **Wither** | 💀 | Noir |
| **Warden** | 👹 | Bleu foncé |

---

### Statuts Possibles

| Statut | Description | Couleur |
|--------|-------------|---------|
| **Stored** | En stockage | Gris |
| **Deployed** | Invoquée (loadout actif) | Vert |
| **Fallen** | Tombée (0 HP) mais stockée | Orange |

---

## ⚙️ Bouton Settings

### Ouvrir Settings

**Clic sur [⚙️ Settings] :**

```
┌──────────────────────────────────────┐
│  Shadow Settings: Zombie_01          │
├──────────────────────────────────────┤
│  Name: [Zombie_01_______] ✏️         │
│                                      │
│  Behavior:                           │
│    ● Defensive                       │
│    ○ Aggressive                      │
│    ○ Passive                         │
│    ○ Hold Position                   │
│                                      │
│  Auto-Deploy (T4 only):              │
│    [ ] When entering combat          │
│                                      │
│  Notes: [__________________]         │
│         [__________________]         │
│                                      │
│     [Cancel]        [Save]           │
└──────────────────────────────────────┘
```

---

### Option : Name (Renommer)

**Champ texte :**

```
Name: [Beru__________] ✏️
```

**Règles :**
- Max 16 caractères
- Lettres, chiffres, underscore
- Pas d'espaces (remplacés par _)
- Pas de caractères spéciaux

**Exemples valides :**
- `Beru`
- `Tank_01`
- `Elite_Knight`
- `Boss_Dragon`

**Le nom apparaît :**
- Au-dessus de l'Ombre en jeu
- Dans le GUI
- Dans les messages de combat

---

### Option : Behavior (Comportement)

**4 modes disponibles :**

#### ● Defensive (Par défaut)

**Comportement :**
- Suit le joueur (10 blocs max)
- Attaque si ennemis < 16 blocs
- Défend le joueur si attaqué
- Reste proche

**Usage :** Exploration, protection générale

---

#### ○ Aggressive

**Comportement :**
- Cherche activement ennemis
- Charge dès détection (32 blocs)
- Ne suit pas nécessairement joueur
- Focus kill rapide

**Usage :** Farm, clear zones, raids

---

#### ○ Passive

**Comportement :**
- Suit uniquement le joueur
- N'attaque JAMAIS (même si frappée)
- Cosmétique pur

**Usage :** Villages (éviter accidents), déplacement pacifique

---

#### ○ Hold Position

**Comportement :**
- Reste en place (ne suit pas)
- Attaque ennemis proches (16 blocs)
- Garde un point fixe

**Usage :** Défense de base, checkpoints, gardien

---

### Option : Auto-Deploy (Shadow Knights uniquement)

**Case à cocher :**

```
[ ] When entering combat
```

**Si cochée :**
- Shadow Knight se déploie automatiquement
- Trigger : Joueur prend dégâts (combat détecté)
- Coût mana : Proportionnel (selon loadout)
- Cooldown : 60 secondes

**Exemple :**
```
Vous explorez → Mob attaque → Vous prenez dégâts
→ Shadow Knight apparaît automatiquement !
→ Vous aide à combattre
```

!!! success "Garde du Corps"
    Activez Auto-Deploy sur vos meilleurs Shadow Knights pour protection 24/7.

---

### Option : Notes

**Champ libre :**

```
Notes: [Bon tank pour boss___]
       [Équipé Sharp V______]
```

**Usage :**
- Mémos personnels
- Stratégies
- Rappels

**Max 100 caractères**

---

## 🎽 Bouton Equipment (Shadow Knights uniquement)

### Interface d'Équipement

**Clic sur [🎽 Equipment] :**

```
┌──────────────────────────────────────┐
│  Equipment: Beru                     │
├──────────────────────────────────────┤
│                                      │
│         [🪖 Helmet Slot]             │
│              Empty                   │
│                                      │
│  [⚔️ Main]   👤   [🛡️ Off]          │
│    Empty          Empty              │
│                                      │
│         [👕 Chestplate]              │
│              Empty                   │
│                                      │
│         [👖 Leggings]                │
│              Empty                   │
│                                      │
│         [👢 Boots]                   │
│              Empty                   │
│                                      │
├──────────────────────────────────────┤
│  Stats Preview:                      │
│  ❤️ HP: 300 (base)                   │
│  ⚔️ ATK: 36 (base)                   │
│  🛡️ DEF: 25 (base)                   │
│  🏃 SPD: 0.33                         │
├──────────────────────────────────────┤
│  Your Inventory:                     │
│  [⚔️] [🪖] [👕] [👖] [👢] [🛡️] ...   │
│                                      │
├──────────────────────────────────────┤
│     [Remove All]    [Save & Close]   │
└──────────────────────────────────────┘
```

---

### Équiper un Item

**Procédure :**

1. **Voir votre inventaire** en bas
2. **Clic gauche** sur item (ex: Netherite Helmet)
3. **Drag** vers slot correspondant (Helmet)
4. **Drop** (relâcher)
5. ✅ **Item équipé !**

**Visuel :**
```
[🪖 Helmet Slot]
   Netherite Helmet
   Protection IV, Unbreaking III
```

---

### Retirer un Item

**Procédure :**

1. **Clic droit** sur slot équipé
2. Item retourne dans inventaire
3. Slot redevient vide

**Alternative :**
- Bouton **[Remove All]** retire tout l'équipement d'un coup

---

### Stats Preview

**Mise à jour en temps réel :**

```
Sans équipement :
❤️ HP: 300
⚔️ ATK: 36
🛡️ DEF: 25

Avec Full Netherite :
❤️ HP: 300 (inchangé)
⚔️ ATK: 36 + 8 (épée) = 44
🛡️ DEF: 25 + 20 (armure) = 45
```

**Calcul dynamique instantané.**

---

### Items Recommandés

**Voir page dédiée :** [Shadow Knights Équipement →](../shadows/shadow-knights.md#équipement)

**TL;DR :**
- **Arme :** Netherite Sword (Sharpness V)
- **Armure :** Full Netherite (Protection IV)
- **Offhand :** Shield OU Totem of Undying

---

## ❌ Bouton Release

### Fonction

**Supprimer définitivement une Ombre.**

---

### Procédure

**Clic sur [❌ Release] :**

```
┌──────────────────────────────────────┐
│  ⚠️ Release Shadow: Zombie_01        │
├──────────────────────────────────────┤
│  This action is PERMANENT.           │
│  You will NOT be able to recover     │
│  this shadow.                        │
│                                      │
│  If this is a Shadow Knight,         │
│  equipment will be returned to       │
│  your inventory.                     │
│                                      │
│  Slots freed: 1                      │
│                                      │
│     [Cancel]        [Confirm]        │
└──────────────────────────────────────┘
```

---

### Confirmation Requise

**Tapez le nom pour confirmer (Tier 4-5 uniquement) :**

```
Type shadow name to confirm: [_______]

(Sécurité pour éviter release accidentel de Shadow Knights/Boss)
```

---

### Conséquences

**Après confirmation :**

1. ✅ Ombre supprimée de l'Army
2. ✅ Slots libérés (1, 2, ou 10)
3. ✅ **Items retournés** (si Shadow Knight)
4. 💬 Message : *"Shadow released: [nom]"*
5. ❌ **Irréversible** (impossible de récupérer)

!!! danger "Attention"
    Release = perte définitive. Vous devrez re-Arise pour en créer une nouvelle.

---

### Quand Release ?

**Situations où c'est utile :**

- 🗑️ **Ombres faibles** (Tier 1 en late-game)
- 📦 **Besoin de slots** (faire de la place pour Boss)
- 🔄 **Remplacer** (version améliorée disponible)
- 🧹 **Nettoyage** (Army encombrée)

**Évitez de release :**
- Shadow Knights équipés (sauf si vraiment inutile)
- Boss Ombres (ultra-rares)
- Ombres nommées/sentimentales

---

## 📊 Statistiques Army

### Panneau de Stats

**En haut de l'onglet :**

```
┌─────────────────────────────────────┐
│  ARMY - 42/100 Slots                │
│                                     │
│  Breakdown:                         │
│  Tier 1: 20 (20 slots)              │
│  Tier 2: 10 (10 slots)              │
│  Tier 3: 5  (5 slots)               │
│  Tier 4: 3  (6 slots)               │
│  Tier 5: 1  (10 slots)              │
│                                     │
│  Total Shadows: 39                  │
│  Currently Deployed: 15             │
│  In Storage: 24                     │
│                                     │
│  Estimated Invoke Cost: 250 mana    │
└─────────────────────────────────────┘
```

**Cliquer dessus pour détails.**

---

## 💡 Actions en Masse

### Sélection Multiple

**Shift+Clic :**
- Sélectionner plusieurs Ombres
- Actions groupées possibles

**Ctrl+A :**
- Sélectionner toutes (filtrées)

---

### Actions Groupées

**Menu contextuel (clic droit sur sélection) :**

```
[Sélection: 5 Ombres]

→ Change Behavior (All to Aggressive)
→ Add to Loadout
→ Release All (avec confirmation)
```

!!! warning "Release All"
    Utilisez avec précaution. Confirmation par nom requis pour chaque Tier 4+.

---

## 🔊 Sons & Feedback

### Sons d'Action

| Action | Son |
|--------|-----|
| **Sélectionner Ombre** | *Ting* |
| **Ouvrir Settings** | *Whoosh* |
| **Équiper item** | *Clank* |
| **Release** | *Fade out* |
| **Save** | *Chime* |

---

### Feedback Visuel

**Hover :**
- Carte Ombre s'illumine (violet)

**Sélection :**
- Bordure violette épaisse

**Modification :**
- Indicateur "💾 Saving..." pendant 1s

---

## ❓ FAQ

### "Je ne trouve pas mon Ombre"

**Solution :**
1. Utiliser barre de recherche
2. Vérifier filtres (peut-être masquée)
3. Tri par "Date Added" (si récente)

---

### "Stats Ombre ont changé"

**Normal !** Stats basées sur VOUS :
- Vous équipez armure → DEF augmente → Ombres aussi
- Vous level up → HP augmente → Ombres aussi

**Les stats sont dynamiques.**

---

### "Ombre déployée mais pas visible en jeu"

**Causes possibles :**
- Ombre tombée (0 HP) → Despawn
- Trop loin (> 64 blocs) → Unload
- Chunk non chargé

**Solution :**
- Rappeler + Réinvoquer (Monarch's Army)

---

## 🎓 Prochaines Étapes

!!! success "Organiser Votre Armée"
    - [Créer des Loadouts →](loadouts.md)
    - [Organiser en Squads →](loadouts.md#squads)
    - [Shadow Knights Détaillés →](../shadows/shadow-knights.md)

---

!!! quote "Conseil"
    *"Une armée bien gérée vaut mieux qu'une armée nombreuse."*