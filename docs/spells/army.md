# ⚔️ Monarch's Army

> *"Mes serviteurs, à moi !"*

**Monarch's Army** est le sort qui invoque ou rappelle votre armée d'Ombres. C'est votre principal outil de combat.

---

## 📊 Informations Générales

| Attribut | Valeur |
|----------|--------|
| **Type** | Invocation / Toggle |
| **Niveaux** | 1 (unique) |
| **Coût mana** | Variable (voir ci-dessous) |
| **Cooldown** | 30 secondes |
| **Cast time** | 3 secondes (invocation) / Instantané (rappel) |

---

## 🎯 Fonction

**Monarch's Army** a **deux fonctions** selon votre situation :

### Mode 1 : Invocation

**Si aucune Ombre n'est invoquée :**
- ✅ Invoque votre **Loadout actif**
- 🌀 Ombres apparaissent en cercle autour de vous
- 📊 Formation selon vos Squads

### Mode 2 : Rappel

**Si des Ombres sont déjà invoquées :**
- ✅ Rappelle **toutes** les Ombres
- ⚡ Instantané (pas de cast time)
- 💾 Ombres retournent en stockage

---

## 💰 Coûts Mana

### Invocation

**Formule :**
```
Coût = 100 + (10 × Nombre d'Ombres)
```

### Exemples

| Nombre d'Ombres | Coût Mana |
|-----------------|-----------|
| 1 | 110 |
| 5 | 150 |
| 10 | 200 |
| 20 | 300 |
| 30 | 400 |
| 50 | 600 |
| 100 | 1100 |

!!! warning "Attention"
    Invoquer 100 Ombres coûte **1100 mana** ! Assurez-vous d'avoir assez (base = 100 mana).

### Rappel

**Coût fixe : 50 mana**

Peu importe le nombre d'Ombres, rappeler coûte toujours 50 mana.

---

## 🎨 Animations

### Invocation

1. **Cast de 3 secondes** (barre de progression)
2. **Portails violets** s'ouvrent en cercle (rayon 5 blocs)
3. **Ombres émergent** simultanément
4. **Formation automatique** selon Squads
5. 💬 Message : *"Shadow Army summoned!"*

**Durée totale :** ~4 secondes

---

### Rappel

1. **Cast instantané** (pas de délai)
2. **Ombres se dissolvent** en particules noires
3. **Retour en stockage**
4. 💬 Message : *"Shadow Army recalled."*

**Durée totale :** ~1 seconde

---

## 📦 Système de Loadout

### Qu'est-ce qu'un Loadout ?

Un **Loadout** est une composition prédéfinie d'Ombres organisées en Squads.

**Caractéristiques :**
- 🎯 **5 Loadouts max** sauvegardables
- 👥 **5 Squads max** par Loadout
- 📊 **100 slots max** par Loadout
- ⚙️ **Configurable** dans Monarch's Domain

### Loadout Actif

**Seul le Loadout actif (coche ●) est invoqué par Monarch's Army.**

**Pour changer de Loadout actif :**
1. Rappeler l'armée actuelle (si invoquée)
2. Entrer dans Monarch's Domain
3. Onglet Loadouts → Sélectionner un autre
4. Sortir et réinvoquer

---

## 👥 Système de Squads

### Qu'est-ce qu'un Squad ?

Un **Squad** est un groupe tactique d'Ombres avec comportement unifié.

**Avantages :**
- 🎯 Commandes de groupe (future feature)
- 📊 Formation coordonnée
- 🧠 AI améliorée (reste groupé)

### Formations de Squad

**Triangle (Recommandé pour combat) :**
```
    🛡️ (Tank)
   ⚔️ ⚔️ (DPS)
  🏹 🏹 🏹 (Ranged)
```

**Line (Bon pour bloquer) :**
```
🛡️ 🛡️ 🛡️ 🛡️ 🛡️
```

**Circle (Focus fire) :**
```
      🎯
   ⚔️  🐉  ⚔️
      ⚔️
```

---

## 🎮 Utilisations Tactiques

### Exploration

**Loadout "Scout" (5-10 Ombres) :**
- Coût : 150-200 mana
- Composition : Tier 1 rapides (Spiders, Skeletons)
- Usage : Exploration, farm mobs basiques

---

### Boss Fights

**Loadout "Raid" (20-30 Ombres) :**
- Coût : 300-400 mana
- Composition :
  - Squad 1 : Tanks (Ravagers, Zombies)
  - Squad 2 : DPS (Shadow Knights, Piglin Brutes)
  - Squad 3 : Support (Skeletons archers)
- Usage : Boss difficiles, raids

---

### Farm Efficace

**Loadout "Farm" (30-50 Ombres) :**
- Coût : 400-600 mana
- Composition : Masse de Tier 1
- Usage : XP farm, loot farm, clear rapide

---

### PvP

**Loadout "War" (50+ Ombres) :**
- Coût : 600+ mana
- Composition :
  - 10 Shadow Knights équipés
  - 10 Tier 3 (tanks)
  - 30 Tier 1-2 (masse)
- Usage : Domination PvP, siège de bases

---

### Endgame

**Loadout "Apocalypse" (50-100 Ombres) :**
- Coût : 600-1100 mana
- Composition :
  - 1-3 Boss (Dragon, Wither, Warden)
  - 10 Shadow Knights full stuff
  - 20 Tier 3
  - Reste en Tier 1-2
- Usage : Détruire tout

---

## 💡 Synergies avec autres Sorts

### Monarch's Army + Monarch Veil

**Combo :**
```
1. Invoquer armée (Monarch's Army)
2. Cast Monarch Veil (buff +50% stats)
3. Ombres deviennent ultra-puissantes
4. Push boss/raid
```

**Résultat :** Puissance × 1.5

---

### Monarch's Army + Monarch Maw

**Combo :**
```
1. Invoquer armée
2. Cast Monarch Maw (debuff ennemis -50%)
3. Ennemis affaiblis, Ombres normales
4. Ratio de force × 2
```

**Résultat :** Victoire facile

---

### Monarch's Army + Monarch Step

**Combo (Tactique) :**
```
1. Invoquer armée
2. Monarch Step (devenir invisible)
3. Ombres combattent (ennemis focus elles)
4. Toi : attaques surprises depuis l'invisible
```

**Résultat :** Damage optimal, survie maximale

---

## ⚠️ Gestion de la Mana

### Problème : Mana insuffisante

**Si 50 Ombres (600 mana) mais vous avez 300 mana max :**

❌ **Impossible d'invoquer** (message : "Not enough mana")

**Solutions :**

#### 1. Réduire le Loadout
- Créer un Loadout "Light" (20 Ombres = 300 mana)
- Utiliser temporairement

#### 2. Augmenter Mana Max
- **Umbral Armor** : +500 mana
- **Monarch Armor** : +600 mana
- **Upgrade Orbs** : +% mana (si implémenté)

#### 3. Potions/Items
- Potions de mana (Iron's Spells)
- Items +mana

#### 4. Invoquer par étapes
- Loadout 1 : 20 Ombres (300 mana)
- Attendre régénération
- Loadout 2 : 20 Ombres supplémentaires
- etc.

---

## 🔧 Upgrade du Sort

**Monarch's Army n'a pas de niveaux.**

Le sort reste identique, mais vous pouvez :
- ✅ Améliorer vos **Loadouts** (plus d'Ombres)
- ✅ Augmenter votre **mana max** (invoquer plus)
- ✅ Réduire cooldown via **achievements** (-5s)

---

## 🎓 Stratégies Avancées

### Switch Loadout Mid-Combat

**Impossible directement.** Vous devez :
1. Rappeler armée (50 mana)
2. Entrer Monarch's Domain
3. Changer Loadout actif
4. Sortir et réinvoquer

**Temps total :** ~30 secondes (+ cooldowns)

!!! tip "Planifier à l'avance"
    Choisissez le bon Loadout AVANT le combat. Switch en combat = risqué.

---

### Rotation de Cooldown

**Si cooldown actif (30s) :**
- ❌ Impossible d'invoquer/rappeler
- ✅ Utilisez ce temps pour repositionner, régénérer HP/mana

**Réduction cooldown :**
- Achievement "Speed Summoner" : -5s (25s)
- Monarch Armor Set Bonus : -20% cooldown (24s)
- **Combiné** : 25s - 20% = 20s cooldown final

---

### Persistence après Mort

**Si vous mourez :**
- ❌ Ombres disparaissent immédiatement (par défaut)
- ✅ **Avec Monarch Armor Set Bonus** : Ombres persistent 60s

**Stratégie :**
```
1. Tu meurs en boss fight
2. Ombres continuent de combattre (60s)
3. Tu respawns
4. TP vers le boss
5. Ombres ont peut-être tué le boss !
```

---

## ❌ Messages d'Erreur

### "No active Loadout selected"
**Cause :** Aucun Loadout actif (pas de coche ●)  
**Solution :** Monarch's Domain → Loadouts → Activer un

### "Not enough mana!"
**Cause :** Mana < coût invocation  
**Solution :** Réduire Loadout ou augmenter mana max

### "Cannot summon in combat"
**Cause :** Aucune (ce sort marche en combat)  
**Solution :** Si message, c'est un bug

### "Cooldown active (Xs remaining)"
**Cause :** Cooldown 30s pas fini  
**Solution :** Attendre

### "Shadow Army already active"
**Cause :** Essayer d'invoquer alors que Ombres déjà invoquées  
**Solution :** Utiliser le sort pour rappeler d'abord

---

## 🎯 Optimisation par Phase de Jeu

### Early Game (Niveau 1-20)

**Loadout :** 5-10 Ombres (150-200 mana)  
**Raison :** Mana limitée, peu d'Ombres disponibles

### Mid Game (Niveau 20-50)

**Loadout :** 20-30 Ombres (300-400 mana)  
**Raison :** Umbral Armor (+500 mana), plus d'Ombres

### Late Game (Niveau 50-80)

**Loadout :** 40-60 Ombres (500-700 mana)  
**Raison :** Monarch Armor (+600 mana), armée complète

### Endgame (Niveau 80+)

**Loadout :** 80-100 Ombres (900-1100 mana)  
**Raison :** Build maxé, mana énorme, domination totale

---

## 💡 Astuces & Conseils

!!! tip "Loadouts multiples"
    Créez plusieurs Loadouts pour différentes situations :
    - Exploration légère (5)
    - Farm moyen (20)
    - Boss fight (40)
    - War ultime (100)

!!! tip "Économie de mana"
    Rappeler (50) puis réinvoquer (100+) coûte cher. Gardez vos Ombres invoquées sauf nécessité.

!!! tip "Combat prolongé"
    Si Ombres tombent à 0 HP (despawn), rappeler + réinvoquer les restaure à 100% HP !

!!! tip "Synchronisation Veil"
    Invoquez → Cast Veil immédiatement → Buff dure 25s → Domination

!!! warning "Lag Warning"
    100 Ombres simultanées = lag potentiel. Testez votre PC. 50 Ombres = plus stable.

---

## 🔗 Voir Aussi

- [Monarch's Domain](domain.md) - Créer vos Loadouts
- [Squads](../domain/loadouts.md) - Organiser tactiquement
- [Monarch Veil](veil.md) - Buff ultime
- [Stratégies](../strategies/builds.md) - Builds optimaux

---

!!! quote "Citation"
    *"Une armée n'est forte que si son général sait la commander."*
