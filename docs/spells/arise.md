# ⚰️ Arise

> *"Lève-toi, mon serviteur."*

**Arise** est le sort signature de la classe Shadow Monarch. Il vous permet de convertir les créatures vaincues en Ombres fidèles.

---

## 📊 Informations Générales

| Attribut | Valeur |
|----------|--------|
| **Type** | Invocation / Necromancy |
| **Niveaux** | 1 → 10 |
| **Coût mana** | 50 → 250 (selon tier) |
| **Cooldown** | 10s → 1s |
| **Cast time** | 2s (instantané niveau 10) |
| **Portée** | 5 → 25 blocs |

---

## 🎯 Fonction

**Arise** convertit un mob mort en Ombre fidèle qui combattra à vos côtés.

### Conditions

Pour utiliser Arise avec succès :

- ✅ Le mob doit être **mort depuis moins de 30 secondes**
- ✅ Le mob doit être dans `mob_tiers.json`
- ✅ Vous devez avoir des **slots libres** (< 100)
- ✅ Vous devez **viser le cadavre** (crosshair)
- ✅ Assez de mana selon le tier

---

## 📈 Progression par Niveau

### Niveau 1 - Débutant

| Stat | Valeur |
|------|--------|
| Tiers accessibles | Tier 1 uniquement |
| Chance de succès | **40%** |
| Coût mana | 50 (T1) |
| Cooldown | 10 secondes |
| Portée | 5 blocs |

!!! warning "Échec possible"
    À ce niveau, Arise échoue 60% du temps. Réessayez jusqu'au succès !

---

### Niveau 2

| Stat | Valeur |
|------|--------|
| Tiers accessibles | Tier 1 |
| Chance de succès | **50%** |
| Coût mana | 50 (T1) |
| Cooldown | 9 secondes |
| Portée | 6 blocs |

---

### Niveau 3 - Élites débloquées

| Stat | Valeur |
|------|--------|
| Tiers accessibles | **Tier 1-2** |
| Chance de succès | **60%** |
| Coût mana | 50 (T1) / 75 (T2) |
| Cooldown | 8 secondes |
| Portée | 7 blocs |

!!! success "Déblocage Tier 2"
    Creepers, Endermen, Vindicators maintenant accessibles !

---

### Niveau 4

| Stat | Valeur |
|------|--------|
| Tiers accessibles | Tier 1-2 |
| Chance de succès | **70%** |
| Coût mana | 50 (T1) / 75 (T2) |
| Cooldown | 7 secondes |
| Portée | 8 blocs |

---

### Niveau 5 - Commandants débloqués

| Stat | Valeur |
|------|--------|
| Tiers accessibles | **Tier 1-2-3** |
| Chance de succès | **80%** |
| Coût mana | 50 (T1) / 75 (T2) / 100 (T3) |
| Cooldown | 6 secondes |
| Portée | 9 blocs |

!!! success "Déblocage Tier 3"
    Ravagers, Piglin Brutes, Evokers maintenant accessibles !

---

### Niveau 6

| Stat | Valeur |
|------|--------|
| Tiers accessibles | Tier 1-2-3 |
| Chance de succès | **85%** |
| Coût mana | 50 (T1) / 75 (T2) / 100 (T3) |
| Cooldown | 5 secondes |
| Portée | 10 blocs |

---

### Niveau 7 - Shadow Knights débloqués

| Stat | Valeur |
|------|--------|
| Tiers accessibles | **Tier 1-2-3-4** |
| Chance de succès | **90%** |
| Coût mana | 50/75/100/**150 (T4)** |
| Cooldown | 4 secondes |
| Portée | 12 blocs |

!!! success "Déblocage Shadow Knights"
    Vous pouvez maintenant Arise des **joueurs morts** ! Équipables et ultra-puissants.

---

### Niveau 8

| Stat | Valeur |
|------|--------|
| Tiers accessibles | Tier 1-2-3-4 |
| Chance de succès | **95%** |
| Coût mana | 50/75/100/150 |
| Cooldown | 3 secondes |
| Portée | 15 blocs |

---

### Niveau 9 - Boss débloqués

| Stat | Valeur |
|------|--------|
| Tiers accessibles | **Tier 1-2-3-4-5** |
| Chance de succès | **98%** |
| Coût mana | 50/75/100/150/**250 (T5)** |
| Cooldown | 2 secondes |
| Portée | 20 blocs |

!!! success "Déblocage Boss"
    Ender Dragon, Wither, Warden maintenant accessibles ! L'ultime puissance.

---

### Niveau 10 - MAÎTRISE PARFAITE

| Stat | Valeur |
|------|--------|
| Tiers accessibles | **TOUS** |
| Chance de succès | **100% (GARANTI)** |
| Coût mana | 50/75/100/150/250 |
| Cooldown | **1 seconde** |
| Portée | **25 blocs** |
| **Bonus** | ⚡ **Instantané** (pas de cast time) |

!!! success "Maîtrise absolue"
    Arise ne peut plus échouer. Cast instantané. C'est la perfection.

---

## 🎨 Animations

### Cast Normal (Tier 1-3)

1. **Main du joueur** s'illumine en violet (2s)
2. **Rayon violet** vers le cadavre
3. **Portail noir** s'ouvre sous le corps (1m diamètre)
4. **Corps aspiré** dans le portail (tourbillon)
5. **Ombre émerge** avec yeux bleus brillants
6. **Particules** violettes/noires autour

**Durée :** ~3 secondes

---

### Cast Shadow Knight (Tier 4)

1-4. Identique (portail 2m)
5. **Shadow Knight émerge** lentement avec équipement
6. **Particules bleues/violettes intenses**
7. **Aura de puissance** autour
8. **Message :** *"A knight rises..."*

**Durée :** ~4 secondes

---

### Cast Boss (Tier 5)

1. **Main violette + noire** (énergie intense, 3s cast)
2. **Rayon épais** vers cadavre
3. **ÉNORME portail** (10m diamètre)
4. 🌍 **Tremblement de sol** (effet caméra)
5. **Boss émerge TRÈS lentement** (dramatique)
6. **Rugissement/cri** caractéristique du boss
7. **Onde de choc visuelle** (particules repoussées)
8. **Yeux bleus massifs** s'allument
9. **Message :** *"A titan has been raised!"*

**Durée :** ~6 secondes

---

### Cast Instantané (Niveau 10)

1. **Portail apparaît instantanément**
2. **Ombre émerge directement**
3. **Aucun cast time**

**Durée :** ~1 seconde

---

## ⚠️ Gestion des Échecs

### Si Arise échoue (niveaux 1-9)

- ❌ **Mana consommée** quand même
- ❌ **Cooldown appliqué**
- ✅ **Cadavre reste 30s de plus** (vous pouvez réessayer)
- 💬 Message : *"Failed to raise shadow..."*
- 🔴 **Particules rouges** (échec visuel)

### Augmenter vos chances

**Niveau du sort :**
- Niveau 1 : 40% → Niveau 10 : 100%

**Aucun autre facteur** n'influence la chance (pas de Looting, pas de niveau joueur, etc.)

---

## 💰 Coûts Mana Détaillés

| Tier | Type | Coût Mana | Exemples |
|------|------|-----------|----------|
| **Tier 1** | Soldats | 50 | Zombie, Skeleton, Spider |
| **Tier 2** | Élites | 75 | Creeper, Enderman, Vindicator |
| **Tier 3** | Commandants | 100 | Ravager, Piglin Brute, Evoker |
| **Tier 4** | Shadow Knights | 150 | Joueurs morts |
| **Tier 5** | Boss | 250 | Dragon, Wither, Warden |

---

## ⏱️ Timer du Cadavre

**30 secondes maximum** après la mort du mob.

### Indicateur Visuel

| Temps écoulé | Visuel |
|--------------|--------|
| **0-10s** | Pulse lent (normal) |
| **10-20s** | Pulse moyen |
| **20-25s** | Pulse rapide (orange) ⚠️ |
| **25-28s** | Pulse très rapide (rouge) 🚨 |
| **28-30s** | Particules rouges qui s'échappent |
| **30s** | 💀 **Disparition** (trop tard) |

### Sons

- **0-20s :** Silence
- **20s :** Son subtil (tic-toc)
- **25s :** Son plus fort (urgence)
- **28s :** Alarme (dernière chance)

---

## 🔧 Upgrade du Sort

### Via Arcane Anvil (Iron's Spells)

**Pour passer de niveau N à N+1 :**

**Ingrédients :**
- 1× Arise Scroll (niveau N)
- 1× Shadow Essence
- 1× INK approprié

**Table de correspondance INK :**

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

**Coût total** pour Arise niveau 10 :
- 9 Shadow Essence
- 3 Uncommon Ink
- 2 Rare Ink
- 2 Epic Ink
- 2 Legendary Ink

---

## 💡 Astuces & Stratégies

### Early Game

!!! tip "Priorité niveau 5"
    Montez Arise niveau 5 en priorité absolue (80% succès + Tier 3).

!!! tip "Farm proche de chez vous"
    Créez une zone de farm près de votre base pour Arise rapidement (pas de transport du cadavre).

### Mid Game

!!! tip "Stockpile Shadow Essence"
    Gardez toujours 5-10 Shadow Essence pour upgrade Arise rapidement.

!!! tip "Équipez Looting"
    Looting III sur votre arme = plus de drops (dont 5% Shadow Essence sur Arise réussi).

### Late Game

!!! tip "Boss farming"
    Niveau 9-10 : Farmez Ender Dragon/Wither/Warden pour Ombres ultra-puissantes.

!!! tip "Niveau 10 = confort ultime"
    100% succès + instantané + 25 blocs portée = qualité de vie maximale.

---

## ❌ Messages d'Erreur

### "This creature cannot be raised as a Shadow"
**Cause :** Mob absent de `mob_tiers.json`  
**Solution :** Ajouter le mob dans le JSON (serveur/datapack)

### "Not enough Shadow Army slots! (100/100)"
**Cause :** Capacité maximale atteinte  
**Solution :** Release des Ombres inutiles via GUI

### "The soul has already departed..."
**Cause :** Cadavre trop vieux (>30s)  
**Solution :** Agir plus vite après le kill

### "Your power is insufficient to raise this creature"
**Cause :** Tier trop élevé pour votre niveau Arise  
**Solution :** Upgrade Arise (ex: Tier 3 nécessite niveau 5+)

### "Not enough mana!"
**Cause :** Mana insuffisante  
**Solution :** Attendre régénération ou boire potion

### "Failed to raise shadow... Try again"
**Cause :** RNG (échec du %age de réussite)  
**Solution :** Réessayer (cadavre reste 30s de plus)

---

## 🎓 Comparaison par Niveau

### Quand upgrade ?

| Niveau Actuel | Problème | Upgrade Prioritaire ? |
|---------------|----------|----------------------|
| **1-2** | Échecs fréquents | ✅ **OUI** (60% échecs) |
| **3-4** | Tier 2 utile | ✅ **OUI** (débloquer élites) |
| **5** | Sweet spot | ⚠️ Optionnel (80% suffit pour mid-game) |
| **6** | Mineure amélioration | ❌ **NON** (priorité autres sorts) |
| **7** | Shadow Knights ! | ✅ **OUI** (game changer) |
| **8** | Mineure amélioration | ❌ **NON** |
| **9** | Boss ! | ✅ **OUI** si prêt pour late-game |
| **10** | Perfection | ✅ **OUI** pour confort ultime |

---

## 🔗 Voir Aussi

- [Système d'Ombres](../shadows/overview.md) - Comprendre les 5 tiers
- [Monarch's Army](army.md) - Invoquer vos Ombres
- [Shadow Knights](../shadows/shadow-knights.md) - Tier 4 détaillé
- [Stratégies Arise](../strategies/arise-tips.md) - Optimiser votre farm

---

!!! quote "Citation"
    *"Arise" - Sung Jin-Woo, Solo Leveling*
