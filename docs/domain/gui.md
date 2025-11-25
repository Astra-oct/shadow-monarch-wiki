# 🖥️ Interface GUI de Monarch's Domain

L'interface graphique (GUI) de Monarch's Domain est votre centre de contrôle pour gérer l'intégralité de votre armée et vos cosmétiques.

---

## 🚪 Ouvrir le GUI

### Accès

**Uniquement dans Monarch's Domain :**

1. 🌌 **Être dans la dimension** (caster Monarch's Domain)
2. ⌨️ **Appuyer sur R** (par défaut, configurable)
3. 🖥️ **GUI s'ouvre** (plein écran)

!!! warning "Restriction"
    Le GUI ne s'ouvre QUE dans Monarch's Domain. Impossible dans l'Overworld.

---

### Raccourci Clavier

**Par défaut :** Touche **R**

**Changer :**
1. Options → Contrôles
2. Catégorie "Shadow Monarch"
3. "Open Domain GUI" → Assigner touche
4. Sauvegarder

**Recommandations :**
- Garder R (proche WASD)
- Alternative : G, V, ou touches souris

---

## 🎨 Vue d'Ensemble du GUI

### Layout Général

```
┌─────────────────────────────────────────────────┐
│  Shadow Monarch - Monarch's Domain              │
├──────┬──────────────────────────────────────────┤
│ 📋   │                                           │
│ ARMY │         Contenu Principal                 │
│      │         (varie selon onglet)              │
│ ⚔️   │                                           │
│LOADS │                                           │
│      │                                           │
│ 👑   │                                           │
│TITLES│                                           │
│      │                                           │
│ 🎭   │                                           │
│CAPES │                                           │
│      │                                           │
├──────┴──────────────────────────────────────────┤
│  Slots: 42/100  |  Mana: 850/1000  |  [Close]  │
└─────────────────────────────────────────────────┘
```

---

### Composants Principaux

#### Barre de Navigation (Gauche)

**4 onglets verticaux :**

| Icône | Nom | Fonction |
|-------|-----|----------|
| 📋 | **ARMY** | Gestion individuelle Ombres |
| ⚔️ | **LOADOUTS** | Créer compositions tactiques |
| 👑 | **TITLES** | Équiper titres cosmétiques |
| 🎭 | **CAPES** | Équiper capes cosmétiques |

**Navigation :**
- Clic sur onglet → Change le contenu
- Onglet actif : Surbrillance violette
- Raccourcis clavier : 1, 2, 3, 4

---

#### Zone de Contenu (Centre)

**Affiche :**
- Liste des Ombres (onglet Army)
- Loadouts sauvegardés (onglet Loadouts)
- Titres disponibles (onglet Titles)
- Capes disponibles (onglet Capes)

**Scrollable** si contenu dépasse l'écran

---

#### Barre d'État (Bas)

**Informations en temps réel :**

```
┌────────────────────────────────────────────┐
│ Slots: 42/100 │ Mana: 850/1000 │ [Close] │
└────────────────────────────────────────────┘
```

| Info | Description |
|------|-------------|
| **Slots** | Ombres utilisées / Max (100) |
| **Mana** | Mana actuel / Max du joueur |
| **[Close]** | Fermer GUI (Esc aussi) |

---

## 📋 Onglet ARMY (Détaillé)

**Voir page dédiée :** [Onglet Army →](army.md)

**Résumé rapide :**
- Liste toutes vos Ombres
- Actions : Settings, Equipment, Release
- Filtres et recherche

---

## ⚔️ Onglet LOADOUTS (Détaillé)

**Voir page dédiée :** [Onglet Loadouts →](loadouts.md)

**Résumé rapide :**
- Créer/modifier Loadouts
- Organiser en Squads
- Activer Loadout pour invocation

---

## 👑 Onglet TITLES (Détaillé)

**Voir page dédiée :** [Onglet Titles →](titles.md)

**Résumé rapide :**
- Liste titres débloqués
- Équiper/retirer titre actif
- Preview en temps réel

---

## 🎭 Onglet CAPES (Détaillé)

**Voir page dédiée :** [Onglet Capes →](capes.md)

**Résumé rapide :**
- Liste capes débloquées
- Équiper/retirer cape active
- Preview 3D rotatif

---

## ⌨️ Contrôles & Raccourcis

### Navigation Générale

| Touche | Action |
|--------|--------|
| **R** | Ouvrir/Fermer GUI |
| **Esc** | Fermer GUI |
| **1-4** | Changer onglet (Army/Loads/Titles/Capes) |
| **Tab** | Cycler entre onglets → |
| **Shift+Tab** | Cycler entre onglets ← |

---

### Dans les Listes

| Touche | Action |
|--------|--------|
| **↑ ↓** | Naviguer liste |
| **Page Up/Down** | Scroll rapide |
| **Home** | Début de liste |
| **End** | Fin de liste |
| **Enter** | Sélectionner élément |

---

### Actions Rapides

| Touche | Action |
|--------|--------|
| **Shift+Clic** | Sélection multiple |
| **Ctrl+Clic** | Ajouter/Retirer sélection |
| **Ctrl+A** | Tout sélectionner |
| **Delete** | Release Ombre (avec confirm) |
| **F2** | Renommer sélectionné |

---

## 🎨 Thème Visuel

### Palette de Couleurs

**Couleurs principales :**

| Élément | Couleur | Hex |
|---------|---------|-----|
| **Background** | Noir/violet foncé | #1a0033 |
| **Panneau** | Violet moyen | #3d1a5c |
| **Texte** | Blanc/bleu clair | #e0e0ff |
| **Accent** | Violet vif | #a855f7 |
| **Success** | Vert | #22c55e |
| **Warning** | Orange | #f97316 |
| **Danger** | Rouge | #ef4444 |

---

### Typographie

**Polices :**
- **Titres** : Minecraft Bold (20px)
- **Corps** : Minecraft Regular (14px)
- **Stats** : Minecraft Mono (12px)

---

### Animations

**Effets :**
- 🌟 **Hover** : Surbrillance douce (0.2s)
- ✨ **Click** : Pulse (0.1s)
- 🌀 **Loading** : Spinner violet
- 💫 **Transition** onglets : Fade (0.3s)

---

## 🔍 Système de Recherche

### Barre de Recherche

**Emplacement :** En haut de chaque onglet avec listes

```
┌─────────────────────────────────────┐
│ 🔍 Search: [_____________]  [x]     │
└─────────────────────────────────────┘
```

---

### Recherche dans ARMY

**Recherche par :**
- **Nom** : "Beru", "Tank"
- **Type** : "Zombie", "Skeleton"
- **Tier** : "1", "T2", "Tier 3"
- **Stats** : "HP>100", "ATK<20"

**Exemples :**
```
"zombie" → Tous les zombies
"tier 4" → Tous Shadow Knights
"HP>200" → Ombres avec HP > 200
```

---

### Filtres Avancés

**Boutons de filtre :**

```
[All] [T1] [T2] [T3] [T4] [T5]
[Stored] [Deployed] [Equipped]
```

**Combinaisons :**
- Tier 2 + Deployed = Ombres T2 actuellement invoquées
- Tier 4 + Equipped = Shadow Knights avec équipement

---

## 📊 Système de Tri

### Options de Tri

**Disponible dans onglets Army et Loadouts :**

```
Sort by: [▼ Alphabetical]
```

**Options :**
- **Alphabetical** (A→Z)
- **Tier** (1→5)
- **Date Added** (récent→ancien)
- **Power** (HP × ATK, décroissant)
- **Slots Used** (croissant)

---

## 💾 Auto-Save

### Fonctionnement

**Tous les changements sont sauvegardés automatiquement :**

- ✅ Modification Loadout → Save instant
- ✅ Release Ombre → Save instant
- ✅ Équiper Title/Cape → Save instant
- ✅ Renommer Ombre → Save après 2s inactivité

**Indicateur :**
```
[💾 Saved] → Apparaît brièvement en haut à droite
```

---

### Sauvegarde Manuelle

**Bouton [Save All] :**
- Bas à droite du GUI
- Force sauvegarde de toutes les modifications
- Utile avant fermeture si lag

---

## 🎮 Interactions Drag & Drop

### Utilisation

**Applicable dans :**
- 📋 Army → Loadouts (ajouter Ombre à Loadout)
- ⚔️ Loadouts → Squads (organiser Ombres)
- 🎽 Equipment Shadow Knights (équiper items)

---

### Procédure

**Exemple : Ajouter Ombre à Loadout**

1. **Onglet ARMY** → Sélectionner Ombre
2. **Clic gauche maintenu** sur l'Ombre
3. **Drag** (glisser) vers onglet LOADOUTS
4. **Passer** à onglet Loadouts (auto-switch)
5. **Drop** (relâcher) dans zone Loadout
6. ✅ Ombre ajoutée !

---

## ⚠️ Messages & Notifications

### Types de Messages

#### Success (Vert)

```
✅ Shadow Knight equipped successfully!
✅ Loadout "Boss Raid" saved!
✅ Title equipped: [Shadow Monarch]
```

---

#### Warning (Orange)

```
⚠️ Loadout exceeds 100 slots (currently 105)
⚠️ Shadow Knight has no weapon equipped
⚠️ This action cannot be undone
```

---

#### Error (Rouge)

```
❌ Not enough slots (100/100)
❌ Cannot release Shadow while deployed
❌ Invalid loadout name
```

---

### Confirmations

**Actions irréversibles demandent confirmation :**

```
┌──────────────────────────────────────┐
│  Release Shadow: "Beru"              │
│                                      │
│  This action is PERMANENT.           │
│  Equipment will be returned.         │
│                                      │
│     [Cancel]        [Confirm]        │
└──────────────────────────────────────┘
```

---

## 🔧 Options du GUI

### Paramètres Disponibles

**Menu Options → Shadow Monarch → GUI :**

| Option | Défaut | Description |
|--------|--------|-------------|
| **GUI Scale** | Auto | Taille interface |
| **Show Tooltips** | ON | Info-bulles hover |
| **Animations** | ON | Effets visuels |
| **Auto-Save** | ON | Sauvegarde auto |
| **Sound Effects** | ON | Sons clic/actions |

---

### GUI Scale

**Options :**
- **Auto** : S'adapte à résolution
- **Small** : 80% taille (écrans 4K)
- **Normal** : 100%
- **Large** : 125% (écrans petits)

---

## 🎵 Sons du GUI

### Sons d'Interface

**Actions sonores :**

| Action | Son |
|--------|-----|
| **Ouvrir GUI** | *Woosh* mystique |
| **Changer onglet** | *Click* doux |
| **Sélectionner Ombre** | *Ting* léger |
| **Équiper item** | *Clank* armure |
| **Release** | *Woosh* disparition |
| **Save** | *Chime* succès |
| **Error** | *Buzz* négatif |

**Volume :** Configurable (Options → GUI → Sound Effects)

---

## 💡 Tips d'Utilisation

### Navigation Rapide

!!! tip "Raccourcis Clavier"
    Utilisez **1, 2, 3, 4** pour switcher onglets instantanément au lieu de cliquer.

!!! tip "Double-Clic"
    Double-clic sur une Ombre ouvre directement son menu Settings.

---

### Organisation

!!! tip "Recherche Fréquente"
    Utilisez la recherche pour trouver rapidement une Ombre spécifique dans une Army de 100.

!!! tip "Filtres Combinés"
    Tier 4 + Equipped = Voir rapidement quels Shadow Knights ont du stuff.

---

### Efficacité

!!! tip "Drag & Drop Multiple"
    Shift+Clic pour sélectionner plusieurs Ombres → Drag tout vers Loadout.

!!! tip "Raccourci F2"
    Sélectionner Ombre → F2 → Renommer directement sans ouvrir Settings.

---

## ❌ Problèmes Fréquents

### "GUI ne s'ouvre pas"

**Causes possibles :**
- ❌ Pas dans Monarch's Domain
- ❌ Keybind pas configuré
- ❌ Conflit avec autre mod

**Solution :**
1. Vérifier dimension (ciel = void noir ?)
2. Options → Contrôles → "Open Domain GUI"
3. Tester sans autres mods

---

### "Changements non sauvegardés"

**Causes possibles :**
- ❌ Auto-Save désactivé
- ❌ Fermeture trop rapide (< 2s)
- ❌ Crash/déconnexion

**Solution :**
1. Activer Auto-Save (Options)
2. Cliquer [Save All] avant fermer
3. Attendre indicateur "💾 Saved"

---

### "Lag dans le GUI"

**Causes possibles :**
- ❌ Beaucoup d'Ombres (90+)
- ❌ Animations ON
- ❌ GUI Scale trop grand

**Solution :**
1. Options → GUI → Animations OFF
2. GUI Scale → Small
3. Fermer/Rouvrir GUI

---

## 🎓 Prochaines Étapes

!!! success "Explorer Chaque Onglet"
    - [Onglet Army Détaillé →](army.md)
    - [Onglet Loadouts Détaillé →](loadouts.md)
    - [Onglet Titles →](titles.md)
    - [Onglet Capes →](capes.md)

---

!!! quote "Conseil"
    *"Un bon Monarch maîtrise son interface. Prenez le temps de l'explorer."*