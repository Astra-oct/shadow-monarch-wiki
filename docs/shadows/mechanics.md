# ⚙️ Mécaniques Avancées des Ombres

Comprendre les mécaniques profondes du système d'Ombres pour optimiser votre gameplay.

---

## 📊 Scaling Dynamique des Stats

### Principe de Base

**Vos Ombres évoluent avec VOUS automatiquement.**

**Formule :**
```
Stat Ombre = Stat Joueur × Coefficient Tier
```

---

### Exemple Concret de Progression

**Vous au niveau 1 :**
```
HP : 20
ATK : 5
DEF : 0
SPD : 0.1

Votre Zombie Ombre :
HP : 20 × 0.8 = 16
ATK : 5 × 0.6 = 3
DEF : 0 × 0.9 = 0
SPD : 0.1 × 0.7 = 0.07
```

**Vous niveau 50 (Full Diamond Armor, Sharp V) :**
```
HP : 100
ATK : 25
DEF : 20
SPD : 0.12

Même Zombie Ombre (automatiquement) :
HP : 100 × 0.8 = 80
ATK : 25 × 0.6 = 15
DEF : 20 × 0.9 = 18
SPD : 0.12 × 0.7 = 0.084
```

**Votre Ombre est 5× plus forte sans rien faire !**

---

### Sources de Stats Joueur

**Ce qui influence vos Ombres :**

| Source | Effet sur Vous | Effet sur Ombres |
|--------|----------------|------------------|
| **Armure** | +DEF | +DEF (selon coeff) |
| **Arme** | +ATK | +ATK (selon coeff) |
| **Enchantements** | +Stats | ✅ Inclus |
| **Potions** | +Stats temporaires | ❌ Non inclus |
| **Beacon** | +Stats temporaires | ❌ Non inclus |
| **Monarch Veil** | Pas de buff | ✅ Buff Ombres |

!!! info "Stats de Base Uniquement"
    Les Ombres utilisent vos stats **permanentes** (équipement, enchants). Les buffs temporaires ne s'appliquent PAS.

---

## 🔄 Système de Respawn

### Mort vs Despawn

**Différence critique :**

| Événement | Résultat |
|-----------|----------|
| **Ombre atteint 0 HP** | Despawn (reste dans Army) |
| **Joueur meurt** | Ombres despawn (restent dans Army) |
| **Joueur déconnexion** | Ombres despawn (restent dans Army) |
| **Release manuelle** | ❌ Suppression définitive |

---

### Cooldown de Réinvocation

**Séquence typique :**

```
T = 0s : Ombre tombe (0 HP)
T = 0s : Despawn automatique
T = 0s : Rappeler Army (50 mana, instantané)
T = 0s : Cooldown Monarch's Army (30s)
T = 30s : Cooldown terminé
T = 30s : Réinvoquer Army (mana variable)
T = 33s : Ombre réapparaît à 100% HP
```

**Temps de "résurrection" : 30 secondes**

---

### Stratégie de Combat

**Utiliser le despawn à votre avantage :**

```
Situation : Boss fight, vos Ombres tombent une par une

Option A (Mauvaise) :
- Laisser tomber sans réagir
- Armée réduite progressivement
- Défaite probable

Option B (Bonne) :
- Dès que 5-10 Ombres tombent
- Rappeler TOUTES les Ombres (50 mana)
- Attendre 30s (kite le boss)
- Réinvoquer à 100% HP
- Armée complète restaurée !
```

---

## 🧠 Intelligence Artificielle

### Niveaux d'AI

**Les Ombres ont 3 niveaux d'AI selon le Tier :**

| Tier | Niveau AI | Caractéristiques |
|------|-----------|------------------|
| **Tier 1** | Basique | Suit, attaque proche |
| **Tier 2-3** | Avancée | Kite, évite AOE simple |
| **Tier 4** | Élite | Évite AOE, utilise terrain |
| **Tier 5** | Boss | Capacités spéciales actives |

---

### Comportements Spécifiques

#### Skeleton / Pillager (Archers)

**AI de Kite :**
1. Détecte ennemi
2. Maintient distance 8-12 blocs
3. Tire flèche/carreau
4. Si ennemi approche → Recule
5. Répète

**Résultat :** DPS constant sans prendre dégâts

---

#### Creeper

**AI d'Explosion :**
1. Détecte ennemi
2. Court vers lui (sprint)
3. Arrivé à 2 blocs → Commence explosion (1.5s)
4. **BOOM** (AOE 3×3)
5. Creeper Ombre survit (ne meurt pas de sa propre explosion)

---

#### Enderman

**AI de Téléportation :**
1. Combat normalement
2. Si projectile entrant → TP esquive
3. Si HP < 50% → TP derrière ennemi
4. Si débordé → TP vers joueur

**Résultat :** Très difficile à tuer

---

#### Shadow Knight

**AI Tactique :**
1. **Priorise cibles faibles** (HP bas)
2. **Évite AOE** (recule avant impact)
3. **Utilise couverture** (piliers, murs)
4. **Protège joueur** (intercept attaques)
5. **Flanking** (attaque par les côtés)

---

### Target Priority (Tous Tiers)

**Ordre d'attaque :**

1. 🎯 **Ennemis attaquant le joueur** (priorité absolue)
2. 🆘 **Ennemis attaquant une Ombre alliée**
3. 👁️ **Mobs hostiles détectés**
4. 🚫 **Ignore mobs passifs**

---

## 💥 Dégâts et Résistances

### Dégâts Infligés

**Formule :**
```
Dégâts finaux = ATK Ombre × Multiplicateurs
```

**Multiplicateurs possibles :**

| Source | Multiplicateur |
|--------|----------------|
| **Crit** | ×1.5 |
| **Backstab** | ×1.2 |
| **Monarch Veil** | ×1.5 (buff) |
| **Enchants arme** (Shadow Knights) | Variable |

---

### Dégâts Reçus

**Formule :**
```
Dégâts reçus = Dégâts bruts × (1 - Réduction DEF)
```

**Réduction DEF :**
```
Si DEF = 10 → Réduction = 10% (×0.9)
Si DEF = 20 → Réduction = 20% (×0.8)
Si DEF = 30 → Réduction = 30% (×0.7)
Max = 80% (DEF 80+)
```

---

### Résistances Spéciales

| Ombre | Résistance | Faiblesse |
|-------|------------|-----------|
| **Zombie** | Résistance knockback | Feu (mais réduit) |
| **Skeleton** | - | Soleil (pas de dégâts, moins efficace) |
| **Spider** | Poison (immune) | - |
| **Creeper** | Explosion (sa propre) | Projectiles |
| **Enderman** | Projectiles (TP) | Eau (évite naturellement) |
| **Wither** | Wither effect (immune) | - |
| **Warden** | Tous effets | Aucune |

---

## 🌍 Interactions Monde

### Pathfinding (Navigation)

**Les Ombres peuvent :**
- ✅ Ouvrir portes (si bois)
- ✅ Monter escaliers/slabs
- ✅ Nager (si nécessaire)
- ✅ Sauter 1 bloc
- ✅ Spider : Escalader murs

**Les Ombres NE PEUVENT PAS :**
- ❌ Ouvrir portes fer
- ❌ Activer leviers/boutons
- ❌ Casser blocs
- ❌ Placer blocs
- ❌ Voler (sauf Dragon, Wither)

---

### Collision avec Entités

**Les Ombres :**
- ✅ Se poussent entre elles (légèrement)
- ✅ Poussent mobs/joueurs
- ✅ Sont poussées par explosions
- ❌ Ne traversent PAS les entités

!!! warning "Saturation"
    50+ Ombres dans un espace 10×10 = embouteillage. Restez en mouvement.

---

### Génération de Lag

**Impact Performance :**

| Nombre Ombres | FPS Impact | Recommandation |
|---------------|------------|----------------|
| **1-10** | Négligeable | Tous PC |
| **10-30** | Faible (~5 FPS) | PC moyen+ |
| **30-50** | Moyen (~15 FPS) | PC correct |
| **50-80** | Élevé (~30 FPS) | PC puissant |
| **80-100** | Très élevé (~50 FPS) | PC ultra |

**Optimisations intégrées :**
- Culling d'entités hors écran
- LOD sur animations lointaines
- Particules réduites si > 30 Ombres

---

## 🎯 Ciblage et Commandes

### Système de Ciblage

**Les Ombres ciblent automatiquement selon :**

1. **Distance** (< 16 blocs par défaut)
2. **Comportement** (Defensive/Aggressive)
3. **Priority** (ennemis du joueur > autres)

---

### Commandes Futures (Plannées)

!!! info "Feature en Développement"
    Ces commandes sont prévues mais pas encore implémentées :

**Commandes par Squad :**
- `/shadow squad <nom> attack <target>`
- `/shadow squad <nom> follow`
- `/shadow squad <nom> hold`

**Commandes individuelles :**
- `/shadow <nom> attack <target>`
- `/shadow <nom> teleport`

---

## 🔄 Synchronisation Client/Serveur

### En Multijoueur

**Chaque joueur voit :**
- ✅ Ses propres Ombres (yeux bleus)
- ✅ Ombres des autres joueurs (yeux bleus)
- ❌ Ne peut PAS contrôler Ombres d'autrui

**Affichage :**
```
Au-dessus de chaque Ombre :
[Nom_Ombre] (Propriétaire: PseudoJoueur)
```

---

### Lag Compensation

**Si lag serveur :**
- Ombres continuent AI côté client (prédiction)
- Resync quand connexion stabilisée
- Si désync trop grande → TP vers position correcte

---

## 💾 Stockage & Données

### Format de Sauvegarde

**Chaque Ombre est sauvegardée avec :**

```json
{
  "id": "zombie_01",
  "type": "minecraft:zombie",
  "tier": 1,
  "owner_uuid": "abc123-...",
  "custom_name": "Tank #1",
  "behavior": "DEFENSIVE",
  "stats": {
    "hp_coefficient": 0.8,
    "atk_coefficient": 0.6,
    "def_coefficient": 0.9,
    "spd_coefficient": 0.7
  },
  "equipment": null,  // Shadow Knights uniquement
  "created_timestamp": 1234567890
}
```

---

### Limites de Stockage

**100 slots = 100 entrées max**

**Taille approximative :**
- 1 Ombre Tier 1 : ~500 bytes
- 1 Shadow Knight équipé : ~2 KB
- 100 Ombres : ~50-200 KB

**Négligeable pour la sauvegarde du monde.**

---

## 🔬 Interactions Avancées

### Avec Autres Mods

**Compatibilité testée :**

| Mod | Compatible ? | Notes |
|-----|--------------|-------|
| **Epic Fight** | ✅ Oui | Ombres utilisent animations vanilla |
| **Better Combat** | ✅ Oui | Ombres non affectées |
| **Lycanites Mobs** | ⚠️ Partiel | Ajouter dans mob_tiers.json |
| **Alex's Mobs** | ✅ Oui | Ajouter dans mob_tiers.json |
| **Ice and Fire** | ⚠️ Partiel | Dragons moddés non supportés (trop complexes) |

---

### Avec Dimensions Moddées

**Les Ombres fonctionnent dans :**
- ✅ Nether
- ✅ End
- ✅ Toutes dimensions moddées (Twilight Forest, etc.)
- ✅ Monarch's Domain (mais n'attaquent rien)

---

## 🎮 Limites Techniques

### Limites Serveur

**Recommandations administrateur :**

```yaml
# config/shadow_monarch.toml
max_shadows_per_player = 100  # Défaut
max_shadows_active_total = 500  # Limite serveur globale
shadow_despawn_on_logout = true  # Despawn si déco
```

---

### Anti-Cheese Intégré

**Protections contre exploits :**

1. **Ombres ne farm pas XP** (joueur doit tuer)
2. **Ombres ne dropent rien** (évite duplication)
3. **Ombres ne peuvent pas être Arise** (pas de récursion)
4. **Cooldowns** empêchent spam invocation
5. **Limite 100 slots** empêche armées infinies

---

## 💡 Tips Mécaniques Avancés

### Optimisation DPS

**Calcul théorique DPS max :**

```
Meilleure composition DPS :
20 Shadow Knights (Netherite Sharp V)
= 20 × (ATK joueur × 1.2 × 1.25) × 2 hits/s
= DPS absolu selon votre équipement

Exemple : Si vous avez 30 ATK
20 Knights = 20 × (30 × 1.2 × 1.25) × 2
          = 1800 dmg/seconde
```

---

### Optimisation Survie

**Meilleure composition tank :**

```
30 Ravagers (Tier 3)
= 30 × (HP joueur × 2) × (DEF joueur × 1.5)

Exemple : Si vous avez 200 HP, 20 DEF
30 Ravagers = 30 × 400 HP × 30 DEF
            = 12000 HP total, 900 DEF combinée
```

**Ces Ravagers peuvent tanker un raid entier.**

---

### Économie d'Actions

**Rotation optimale combat long :**

```
1. Invoquer armée (300 mana)
2. Cast Monarch Veil (250 mana)
3. Cast Monarch Maw (100 mana)
4. Combat 25s (Veil actif)
5. Veil expire, Maw encore actif (14s)
6. Maw expire
7. Attendre 15s (cooldowns)
8. Rappeler + Réinvoquer (si Ombres tombées)
9. Répéter
```

---

## 🎓 Prochaines Étapes

!!! success "Maîtriser les Ombres"
    - [Shadow Knights Détaillés →](shadow-knights.md)
    - [Stratégies de Combat →](../strategies/combos.md)
    - [Builds Optimaux →](../strategies/builds.md)

---

!!! quote "Maxime"
    *"Comprendre les mécaniques, c'est doubler la puissance de votre armée."*