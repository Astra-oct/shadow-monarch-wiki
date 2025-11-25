# 🩸 Monarch Blend

> *"Que ton sang nourrisse les ombres."*

**Monarch Blend** est un sort d'attaque qui inflige un puissant effet de saignement stackable : **"Blood of the Monarch"**.

---

## 📊 Informations Générales

| Attribut | Valeur |
|----------|--------|
| **Type** | Attaque / DoT (Damage over Time) |
| **Niveaux** | 1 → 10 |
| **Coût mana** | 30 → 60 |
| **Cooldown** | 1s → 0.5s |
| **Cast time** | Instantané |
| **Portée** | ~15 blocs (projectile) |

---

## 🎯 Fonction

**Monarch Blend** lance un projectile qui inflige des dégâts immédiats et applique l'effet **"Blood of the Monarch"**.

### Blood of the Monarch

**Effet de saignement stackable :**
- 🩸 **Dégâts par seconde** (DoT)
- 📊 **Stacks cumulables** (jusqu'à 10)
- 💊 **Réduit healing** reçu (-10% par stack)
- 💀 **Hemorrhage** : Double DoT à 10 stacks

---

## 📈 Progression par Niveau

### Tableau Complet

| Niveau | Dégâts Initiaux | DoT | Durée | Stacks Max | Mana | CD |
|--------|-----------------|-----|-------|------------|------|-----|
| **1** | 100% ATK | 5 HP/s | 5s | 3 | 30 | 1s |
| **2** | 110% ATK | 6 HP/s | 5.5s | 4 | 33 | 0.9s |
| **3** | 120% ATK | 7 HP/s | 6s | 5 | 36 | 0.9s |
| **4** | 130% ATK | 8 HP/s | 6.5s | 6 | 39 | 0.8s |
| **5** | 150% ATK | 10 HP/s | 8s | 5 | 40 | 1s |
| **6** | 160% ATK | 12 HP/s | 8.5s | 7 | 45 | 0.8s |
| **7** | 170% ATK | 14 HP/s | 9s | 8 | 50 | 0.7s |
| **8** | 180% ATK | 16 HP/s | 9.5s | 9 | 55 | 0.6s |
| **9** | 190% ATK | 18 HP/s | 9.5s | 10 | 58 | 0.5s |
| **10** | 200% ATK | 20 HP/s | 10s | 10 | 60 | 0.5s |

### Calcul des Dégâts Totaux

**Exemple avec niveau 10 :**
```
Dégâts initiaux : 20 ATK × 2.0 = 40 dmg
DoT (1 stack) : 20 HP/s × 10s = 200 dmg
DoT (10 stacks) : 200 × 10 = 2000 dmg

Total (10 stacks) : 40 + 2000 = 2040 dmg
```

**Avec Hemorrhage (10 stacks) :**
```
DoT double : 40 HP/s × 10s = 400 dmg/stack
Total : 40 + 4000 = 4040 dmg
```

**C'est ÉNORME pour un sort avec 0.5s cooldown !**

---

## 🎨 Animations & Visuels

### Cast

1. **Projectile rouge/noir** se forme
2. **Lance vers la cible** (vitesse moyenne)
3. **Impact sanglant** avec particules

---

### Effet "Blood of the Monarch"

**Sur la cible :**
- 🩸 **Sang noir** s'écoule du corps
- 💀 **Particules rouges/noires** constantes
- 📊 **Compteur de stacks** au-dessus de la tête

**Compteur visuel :**
```
[Blood of the Monarch: 5 stacks]
```

---

### Hemorrhage (10 stacks)

**Effet visuel amplifié :**
- 💥 **Explosion de sang noir** à l'application
- 🌊 **Vague de sang** qui pulse
- 💀 **Crânes noirs** flottent autour
- 🚨 **Message** : *"HEMORRHAGE!"*

---

## 💡 Mécaniques Spéciales

### Stacks Cumulables

**Chaque hit de Monarch Blend ajoute 1 stack.**

**Exemple :**
```
Hit 1 : 1 stack (20 HP/s pendant 10s)
Hit 2 : 2 stacks (40 HP/s pendant 10s)
...
Hit 10 : 10 stacks (200 HP/s → 400 HP/s avec Hemorrhage)
```

**Timer refresh :** Chaque nouveau hit reset la durée à 10s.

---

### Réduction Healing

**Chaque stack réduit le healing reçu de 10%.**

```
1 stack : -10% healing
5 stacks : -50% healing
10 stacks : -100% healing (aucun heal possible)
```

**Applications :**
- Boss qui se régénère → Impossible avec 10 stacks
- PvP contre joueurs avec potions → Potions inutiles
- Regen passive → Annulée

---

### Hemorrhage (10 stacks)

**À 10 stacks, le DoT DOUBLE automatiquement.**

```
Normal : 20 HP/s
Hemorrhage : 40 HP/s
```

**Durée :** Jusqu'à expiration du timer (10s)

**Visuel :** Message + effets amplifiés

---

### Persistence après Mort

**Si vous mourez, le saignement CONTINUE jusqu'à expiration.**

**Exemple :**
```
1. Vous appliquez 10 stacks (400 HP/s, 10s)
2. Vous mourez (0:05s écoulées)
3. Boss continue de saigner (5s restantes)
4. Boss perd 400 × 5 = 2000 HP
5. Peut tuer le boss même mort !
```

---

### Ombres ne Peuvent PAS Infliger

**Les Ombres n'appliquent PAS "Blood of the Monarch".**

**Raison :** Trop OP, balance du jeu

**Seul le joueur** peut infliger cet effet.

---

## 🎯 Utilisations Tactiques

### Boss Fights

**Stratégie DoT Stack :**

```
1. Spam Monarch Blend (0.5s CD niveau 10)
2. Atteindre 10 stacks rapidement (~5 secondes)
3. Hemorrhage activé (400 HP/s)
4. Boss perd 4000 HP en 10s
5. Refresh stacks avant expiration
6. Répéter jusqu'à mort
```

**Résultat :** DPS constant sans risque (projectile ranged)

---

### PvP (Combat Joueur)

**Stratégie Anti-Heal :**

```
1. Hit adversaire 10× (10 stacks)
2. -100% healing reçu
3. Potions inutiles
4. Régénération annulée
5. Hemorrhage (400 HP/s) = mort garantie
```

**Résultat :** Aucune échappatoire

---

### Mobs Elite/Mini-Boss

**Stratégie Kite :**

```
1. Garder distance (15 blocs)
2. Spam Blend jusqu'à 10 stacks
3. Reculer pendant que DoT travaille
4. Refresh stacks à 2s restantes
5. Mob ne vous touche jamais
```

**Résultat :** Kill sans dégâts pris

---

## 🔄 Combos avec Autres Sorts

### Blend + Monarch Maw

**Combo "Amplified Bleed" :**

```
1. Cast Monarch Maw (ennemis -50% DEF)
2. Spam Monarch Blend (10 stacks)
3. DoT amplifié par -DEF
4. Mort ultra-rapide
```

**Synergie :** Debuff DEF → DoT plus efficace

---

### Blend + Monarch Step

**Combo "Assassin Bleed" :**

```
1. Monarch Step (invisible)
2. Approche boss
3. Spam Blend pendant invisibilité (10 stacks)
4. Step away avant fin invi
5. Boss meurt du DoT, vous êtes sauf
```

**Synergie :** Sécurité + DPS

---

### Blend + Monarch Reaver

**Combo "Blood Storm" :**

```
1. Spam Blend (10 stacks = 400 HP/s)
2. Attaques mêlée (Monarch Reaver = 14 dmg/hit)
3. Chaque hit Reaver restaure 2% mana (spam Blend infini)
4. DoT + Mêlée = DPS insane
```

**Synergie :** Sustain mana + double source dégâts

---

## 💰 Coût/Bénéfice par Niveau

| Niveau | Mana/Stack | Temps 10 Stacks | Total Mana | DoT Total (10s) |
|--------|------------|-----------------|------------|-----------------|
| 1 | 30 | 3s (max 3) | 90 | 150 HP |
| 5 | 40 | 5s | 200 | 500 HP |
| 10 | 60 | 5s | 600 | 2000 HP (4000 Hemorrhage) |

**Efficacité niveau 10 :**
- 600 mana → 4000 dmg
- **Ratio : 6.66 dmg/mana**
- Meilleur que la plupart des sorts directs

---

## 🔧 Upgrade du Sort

### Via Arcane Anvil

| Upgrade | INK Requis |
|---------|------------|
| 1 → 2 | Uncommon Ink |
| 2 → 3 | Uncommon Ink |
| 3 → 4 | Uncommon Ink |
| 4 → 5 | Rare Ink |
| 5 → 6 | Rare Ink |
| 6 → 7 | Epic Ink |
| 7 → 8 | Epic Ink |
| 8 → 9 | Legendary Ink |
| 9 → 10 | Legendary Ink |

**Coût total niveau 10 :**
- 9 Shadow Essence
- 3 Uncommon Ink
- 2 Rare Ink
- 2 Epic Ink
- 2 Legendary Ink

---

## 🎓 Stratégies Avancées

### Gestion des Stacks

**Timer management :**

```
Stack 1-9 : Spam rapide (5s pour 10 stacks)
Stack 10 : Hemorrhage activé
Seconde 8 : Refresh 1 stack (reset timer à 10s)
Seconde 18 : Refresh à nouveau
Répéter indéfiniment
```

**Résultat :** Hemorrhage permanent avec refresh minimal

---

### Multi-Target

**Si plusieurs ennemis :**

```
Option A : Focus 1 cible (10 stacks → mort)
Option B : 5 stacks sur 2 cibles (spread DoT)
Option C : 3 stacks sur 3 cibles (AOE damage)
```

**Recommandation :** Focus 1 (Hemorrhage >> spread)

---

### Boss Multi-Phase

**Si boss immunité/phases :**

```
Phase vulnerable : Stack 10 → Hemorrhage
Phase immune : Attendre (DoT continue !)
Phase 2 : Re-stack si stacks expirés
```

**Astuce :** Si boss immune pendant Hemorrhage, vous gagnez DPS gratuit

---

## 💡 Astuces & Conseils

!!! tip "Niveau 10 = must-have"
    0.5s CD + 10 stacks + Hemorrhage = DPS optimal. Priorité upgrade.

!!! tip "Kite bosses"
    Blend = ranged. Stack 10 → Reculer → Boss meurt sans vous toucher.

!!! tip "PvP instant-win"
    10 stacks + -100% healing = adversaire condamné. Aucune contre-stratégie.

!!! tip "Persistence post-mortem"
    Stack boss avant de mourir = peut tuer boss après votre mort.

!!! warning "Mana intensive"
    10 stacks niveau 10 = 600 mana. Gardez mana pour ça avant boss fight.

---

## 🆚 Comparaison DoT

### Monarch Blend vs Poison (Vanilla)

| Critère | Blend (10 stacks) | Poison II |
|---------|-------------------|-----------|
| **DoT** | 400 HP/s (Hemorrhage) | 1.2 HP/s |
| **Durée** | 10s (refresh) | 20s |
| **Total dmg** | 4000+ | 24 |
| **Réduit healing** | -100% | Non |

**Verdict :** Blend >>> Poison (333× plus puissant)

---

## ❌ Messages d'Erreur

### "Not enough mana"
**Cause :** Mana < 30-60  
**Solution :** Attendre régénération

### "Target out of range"
**Cause :** Cible > 15 blocs  
**Solution :** Approcher

### "Cooldown active"
**Cause :** CD 0.5-1s pas fini  
**Solution :** Attendre (très court)

---

## 📊 Cas d'Usage Optimaux

| Situation | Recommandation |
|-----------|----------------|
| **Boss HP élevé** | ⭐⭐⭐⭐⭐ (DoT massif) |
| **PvP** | ⭐⭐⭐⭐⭐ (anti-heal crucial) |
| **Mobs élites** | ⭐⭐⭐⭐ (excellent) |
| **Farming mobs faibles** | ⭐⭐ (overkill, coût mana) |
| **Exploration** | ⭐⭐⭐ (bon mais mana intensif) |

---

## 🔗 Voir Aussi

- [Monarch Maw](maw.md) - Combo debuff DEF
- [Monarch Step](step.md) - Kite en sécurité
- [Monarch Reaver](../equipment/weapons.md) - Sustain mana
- [Boss Strategies](../strategies/boss-fights.md) - Vaincre boss

---

!!! quote "Citation"
    *"Le sang de mes ennemis nourrit les ténèbres."*
