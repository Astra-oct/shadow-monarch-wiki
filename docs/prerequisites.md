# ⚙️ Prérequis

Avant de pouvoir jouer avec **Shadow Monarch**, assurez-vous d'avoir tous les éléments nécessaires.

---

## 🎮 Version Minecraft

| Composant | Version Requise |
|-----------|----------------|
| **Minecraft Java Edition** | 1.21.1 |
| **Mod Loader** | NeoForge (dernière version) |

!!! warning "Version Exacte"
    Shadow Monarch est conçu UNIQUEMENT pour Minecraft 1.21.1. Les versions antérieures ou ultérieures ne sont pas supportées.

---

## 📦 Mods Requis

### Iron's Spells and Spellbooks

**Obligatoire** - Shadow Monarch est une extension de ce mod.

- 📥 **Téléchargement :** [CurseForge](https://www.curseforge.com/minecraft/mc-mods/irons-spells-n-spellbooks) ou [Modrinth](https://modrinth.com/mod/irons-spells-n-spellbooks)
- ⚙️ **Version :** Dernière version compatible 1.21.1
- 📖 **Pourquoi :** Fournit le système de sorts, Spell Books, Scroll Forge, Inscription Table, Arcane Anvil

!!! info "Dépendance Critique"
    Sans Iron's Spells, Shadow Monarch ne se lancera PAS. C'est la base du système de magie.

---

### Curios API

**Obligatoire** - Gère les accessoires (Monarch's Seal).

- 📥 **Téléchargement :** [CurseForge](https://www.curseforge.com/minecraft/mc-mods/curios) ou [Modrinth](https://modrinth.com/mod/curios)
- ⚙️ **Version :** Dernière version compatible 1.21.1 + NeoForge
- 📖 **Pourquoi :** Permet d'équiper jusqu'à 10 rings (Monarch's Seal)

!!! info "Slots Rings"
    Shadow Monarch ajoute automatiquement 10 slots "ring" via Curios API.

---

## 🔧 Installation

### Étape 1 : Installer NeoForge

1. Télécharger **NeoForge Installer** pour 1.21.1 : [neoforged.net](https://neoforged.net/)
2. Lancer l'installer
3. Sélectionner "Install Client"
4. Lancer Minecraft avec le profil NeoForge

### Étape 2 : Installer les Mods

1. Télécharger les mods requis :
   - Iron's Spells and Spellbooks
   - Curios API
   - Shadow Monarch

2. Placer les fichiers `.jar` dans le dossier `mods/` :
   ```
   .minecraft/
   └── mods/
       ├── irons_spells_n_spellbooks-1.21.1-x.x.x.jar
       ├── curios-neoforge-1.21.1-x.x.x.jar
       └── shadow_monarch-1.21.1-x.x.x.jar
   ```

3. Lancer Minecraft avec le profil NeoForge

### Étape 3 : Vérification

**Dans le menu principal :**
- Cliquer sur "Mods"
- Vérifier que les 3 mods apparaissent :
  - ✅ Iron's Spells and Spellbooks
  - ✅ Curios API
  - ✅ Shadow Monarch

**En jeu :**
- Taper `/irons_spellbooks version` → Doit afficher la version
- Ouvrir inventaire → Bouton Curios doit être présent

---

## 💻 Configuration Système Recommandée

### Configuration Minimale

| Composant | Minimum |
|-----------|---------|
| **CPU** | Intel Core i5 / AMD Ryzen 5 |
| **RAM** | 6 GB alloués à Minecraft |
| **GPU** | GTX 960 / RX 560 |
| **Stockage** | 2 GB disponibles |

### Configuration Recommandée

| Composant | Recommandé |
|-----------|-----------|
| **CPU** | Intel Core i7 / AMD Ryzen 7 |
| **RAM** | 8-12 GB alloués à Minecraft |
| **GPU** | GTX 1660 / RX 5600 XT |
| **Stockage** | SSD avec 5 GB disponibles |

!!! warning "Performance"
    Invoquer 100 Ombres simultanément peut être exigeant. Configuration recommandée fortement conseillée pour le late-game.

---

## 🔍 Allocation de RAM

**Comment augmenter la RAM allouée à Minecraft :**

### Via le Launcher Officiel

1. Ouvrir le launcher Minecraft
2. Aller dans "Installations"
3. Cliquer sur "..." à côté du profil NeoForge
4. Sélectionner "Modifier"
5. Cliquer sur "Plus d'options"
6. Modifier `-Xmx2G` en `-Xmx8G` (pour 8 GB)
7. Sauvegarder

### Valeurs Recommandées

| Situation | RAM à Allouer |
|-----------|---------------|
| **Exploration légère** | 4-6 GB |
| **Mid-game (20-50 Ombres)** | 6-8 GB |
| **Late-game (50-100 Ombres)** | 8-12 GB |
| **Avec shaders/autres mods** | 10-16 GB |

!!! tip "Sweet Spot"
    8 GB de RAM est le meilleur compromis pour la plupart des joueurs.

---

## 🎮 Contrôles par Défaut

### Sorts (Iron's Spells)

| Action | Touche |
|--------|--------|
| **Ouvrir Spell Book** | Clic droit avec Spell Book équipé |
| **Caster Sort 1** | R (par défaut) |
| **Caster Sort 2** | V (par défaut) |
| **Caster Sort 3-8** | Configurable |

### Shadow Monarch Spécifique

| Action | Touche |
|--------|--------|
| **Ouvrir GUI Domain** | R (dans Monarch's Domain) |
| **Caster Arise** | Défini dans Spell Book |
| **Caster Monarch's Army** | Défini dans Spell Book |

!!! info "Configurable"
    Tous les contrôles peuvent être modifiés dans Options → Contrôles.

---

## 🗺️ Worldgen (Génération de Monde)

### Nouveau Monde Recommandé

**Pour une expérience optimale :**
- ✅ Créer un **nouveau monde** après installation
- ✅ Type : Normal (Overworld classique)
- ✅ Structures : Activées (pour Ancient Cities)

### Monde Existant

**Si vous jouez sur un monde existant :**
- ⚠️ Les nouvelles structures (Ancient Cities) n'apparaîtront que dans les chunks non générés
- ✅ Explorez de nouvelles zones pour trouver Echo Shards

---

## 🔗 Mods Optionnels Recommandés

### Performance

| Mod | Utilité |
|-----|---------|
| **Embeddium** | Optimisation graphique (Sodium pour Forge) |
| **FerriteCore** | Réduction utilisation RAM |
| **ModernFix** | Optimisations générales |

### QoL (Quality of Life)

| Mod | Utilité |
|-----|---------|
| **JEI (Just Enough Items)** | Voir les recettes de craft |
| **JourneyMap** | Minimap + carte du monde |
| **Waystones** | Téléportation rapide |

!!! success "Compatibilité"
    Shadow Monarch est compatible avec la plupart des mods populaires.

---

## ❓ Problèmes Fréquents

### "Shadow Monarch ne se lance pas"

**Causes possibles :**
- ❌ Iron's Spells absent ou mauvaise version
- ❌ Curios API absent
- ❌ Version Minecraft incorrecte (pas 1.21.1)
- ❌ NeoForge pas à jour

**Solution :** Vérifier les logs (`latest.log`) pour identifier le mod manquant.

---

### "Crash au lancement"

**Causes possibles :**
- ❌ Conflit avec un autre mod
- ❌ RAM insuffisante (< 4 GB)
- ❌ Java obsolète

**Solution :**
1. Mettre à jour Java : [java.com](https://www.java.com/)
2. Augmenter la RAM allouée
3. Tester avec seulement Iron's Spells + Curios + Shadow Monarch

---

### "Les sorts ne fonctionnent pas"

**Causes possibles :**
- ❌ Spell Book pas équipé
- ❌ Sort pas appris (Inscription Table)
- ❌ Mana insuffisante
- ❌ Keybind pas configuré

**Solution :** Voir [Guide de Démarrage](getting-started.md) pour apprendre les sorts.

---

## 🎓 Prêt à Commencer ?

Une fois tous les prérequis installés et vérifiés :

!!! success "Étape Suivante"
    [Commencer le Guide de Démarrage →](getting-started.md){ .md-button .md-button--primary }

---

## 🔗 Liens Utiles

- 📥 [Télécharger Shadow Monarch](#)
- 📖 [Documentation Iron's Spells](https://docs.irons-spells.com/)
- 💬 [Discord Shadow Monarch](#)
- 🐛 [Signaler un bug](#)

---

!!! quote "Note"
    *Si vous rencontrez des problèmes d'installation, rejoignez notre Discord pour obtenir de l'aide de la communauté !*