# ⚙️ Configuration

Guide complet pour configurer Shadow Monarch selon vos préférences.

---

## 📁 Emplacement des Fichiers

### Client (Solo)

```
.minecraft/
└── config/
    └── shadowmonarch/
        ├── shadowmonarch-common.toml
        ├── shadowmonarch-client.toml
        └── mob_tiers.json
```

### Serveur

```
server/
└── config/
    └── shadowmonarch/
        ├── shadowmonarch-common.toml
        ├── shadowmonarch-server.toml
        └── mob_tiers.json
```

---

## 🔧 Configuration Commune (Common)

**Fichier :** `shadowmonarch-common.toml`

Ce fichier contient les paramètres partagés entre client et serveur.

### Exemple de Configuration

```toml
[general]
    # Nombre maximum d'Ombres dans l'armée
    # Min: 20, Max: 200, Default: 100
    maxShadowSlots = 100
    
    # Nombre maximum d'Ombres invocables simultanément
    # Min: 10, Max: 50, Default: 20
    maxSummonedShadows = 20
    
    # Les Ombres causent-elles des dégâts de griefing ?
    # Default: false (IMPORTANT: gardez false !)
    shadowsGriefing = false
    
    # Multiplicateur de stats des Ombres
    # Min: 0.5, Max: 2.0, Default: 1.0
    shadowStatsMultiplier = 1.0

[arise]
    # Coût en mana du sort Arise
    # Min: 10, Max: 200, Default: 50
    ariseMana cost = 50
    
    # Cooldown d'Arise (en secondes)
    # Min: 1, Max: 60, Default: 5
    ariseCooldown = 5
    
    # Chance de réussite d'Arise (%)
    # Min: 50, Max: 100, Default: 100
    ariseSuccessRate = 100

[domain]
    # Temps de téléportation vers Domain (secondes)
    # Min: 0, Max: 10, Default: 2
    domainTeleportTime = 2
    
    # Coût mana pour entrer dans Domain
    # Min: 0, Max: 100, Default: 25
    domainManaCost = 25
    
    # Nombre de loadouts maximum
    # Min: 1, Max: 10, Default: 5
    maxLoadouts = 5

[combat]
    # Les Ombres attaquent-elles les autres Ombres ?
    # Default: false
    shadowVsShadow = false
    
    # Multiplicateur dégâts PvP des Ombres
    # Min: 0.1, Max: 2.0, Default: 0.75
    pvpDamageMultiplier = 0.75
    
    # Multiplicateur dégâts PvE des Ombres
    # Min: 0.5, Max: 2.0, Default: 1.0
    pveDamageMultiplier = 1.0

[drops]
    # Chance de drop Monarch's Seal (%)
    # Min: 0.1, Max: 10.0, Default: 0.5
    sealDropChance = 0.5
    
    # Multiplicateur XP des Ombres
    # Min: 0.0, Max: 2.0, Default: 0.5
    shadowXPMultiplier = 0.5
    
    # Les Ombres drop-elles du loot ?
    # Default: true
    shadowsDropLoot = true

[performance]
    # Limite de rendu des Ombres (distance)
    # Min: 16, Max: 128, Default: 64
    shadowRenderDistance = 64
    
    # Afficher les particules des Ombres ?
    # Default: true
    shadowParticles = true
    
    # Limite FPS des animations d'Ombres
    # Min: 15, Max: 60, Default: 30
    shadowAnimationFPS = 30
```

---

## 🖥️ Configuration Client

**Fichier :** `shadowmonarch-client.toml`

Paramètres visuels et interface (client uniquement).

### Exemple de Configuration

```toml
[visuals]
    # Afficher les noms des Ombres au-dessus
    # Default: true
    showShadowNames = true
    
    # Afficher les barres de vie des Ombres
    # Default: true
    showShadowHealthBars = true
    
    # Couleur de l'aura des Ombres (HEX)
    # Default: "#9b59b6" (violet)
    shadowAuraColor = "#9b59b6"
    
    # Opacité de l'aura (%)
    # Min: 0, Max: 100, Default: 80
    shadowAuraOpacity = 80

[gui]
    # Position du compteur d'Ombres (x, y)
    # Default: 10, 10 (haut-gauche)
    shadowCounterX = 10
    shadowCounterY = 10
    
    # Taille de l'interface Domain
    # Options: "small", "medium", "large"
    # Default: "medium"
    domainGUISize = "medium"
    
    # Thème de l'interface
    # Options: "dark", "light", "purple"
    # Default: "purple"
    guiTheme = "purple"

[hotkeys]
    # Touches par défaut (modifiables in-game)
    # Domain Access: "N"
    # Quick Summon: "R"
    # Recall Shadows: "X"
    
[sounds]
    # Volume des sons du mod (%)
    # Min: 0, Max: 100, Default: 100
    modSoundsVolume = 100
    
    # Son d'Arise activé ?
    # Default: true
    ariseSound = true
    
    # Son de téléportation Domain ?
    # Default: true
    domainTeleportSound = true
```

---

## 🌐 Configuration Serveur

**Fichier :** `shadowmonarch-server.toml`

Paramètres serveur (multijoueur uniquement).

### Exemple de Configuration

```toml
[server]
    # Les joueurs peuvent-ils PvP avec Ombres ?
    # Default: true
    allowPvP = true
    
    # Nombre d'Ombres max par joueur (override common)
    # Min: 20, Max: 200, Default: 100
    perPlayerShadowLimit = 100
    
    # Limite globale d'Ombres sur le serveur
    # Min: 100, Max: 5000, Default: 1000
    globalShadowLimit = 1000

[protection]
    # Les Ombres respectent-elles les claims ?
    # Default: true (recommandé)
    respectClaims = true
    
    # Plugins de claim supportés
    # Options: "GriefPrevention", "WorldGuard", "Towny", "Factions"
    claimPlugins = ["GriefPrevention", "WorldGuard"]
    
    # Les Ombres peuvent-elles attaquer dans spawn ?
    # Default: false
    allowSpawnCombat = false

[economy]
    # Coût en $ pour invoquer (Vault requis)
    # Min: 0, Max: 10000, Default: 0
    summonCost = 0
    
    # Coût en $ pour accéder Domain
    # Min: 0, Max: 1000, Default: 0
    domainAccessCost = 0

[moderation]
    # Log toutes les actions Shadow Monarch ?
    # Default: true
    logShadowActions = true
    
    # Cooldown global d'invocation (secondes)
    # Min: 0, Max: 300, Default: 30
    globalSummonCooldown = 30
    
    # Ban certains mobs de conversion ?
    # Format: ["minecraft:villager", "minecraft:iron_golem"]
    bannedMobs = []
```

---

## 📜 Registry Custom (mob_tiers.json)

**Fichier :** `mob_tiers.json`

Définit les Tiers de chaque mob convertible.

### Structure JSON

```json
{
  "mob_tiers": {
    "minecraft:zombie": {
      "tier": 1,
      "stats_multiplier": 1.0,
      "special_abilities": []
    },
    "minecraft:skeleton": {
      "tier": 1,
      "stats_multiplier": 1.0,
      "special_abilities": ["archer"]
    },
    "minecraft:enderman": {
      "tier": 3,
      "stats_multiplier": 1.5,
      "special_abilities": ["teleport", "water_damage"]
    },
    "minecraft:iron_golem": {
      "tier": 3,
      "stats_multiplier": 2.0,
      "special_abilities": ["knockback"]
    },
    "minecraft:ravager": {
      "tier": 5,
      "stats_multiplier": 2.5,
      "special_abilities": ["roar", "stomp"]
    }
  },
  "modded_mobs": {
    "alexsmobs:grizzly_bear": {
      "tier": 2,
      "stats_multiplier": 1.2,
      "special_abilities": ["strength"]
    },
    "mowziesmobs:ferrous_wroughtnaut": {
      "tier": 5,
      "stats_multiplier": 3.0,
      "special_abilities": ["armor", "resistance"]
    }
  }
}
```

### Ajouter un Mob Custom

```json
{
  "mon_mod:mon_mob": {
    "tier": 2,
    "stats_multiplier": 1.3,
    "special_abilities": ["custom_ability"]
  }
}
```

**Après modification :**
1. Sauvegardez le fichier
2. Relancez Minecraft
3. Testez la conversion in-game

---

## 🎮 Configurations Recommandées

### Pour Solo (Performance Maximale)

```toml
maxSummonedShadows = 15
shadowRenderDistance = 48
shadowAnimationFPS = 20
shadowParticles = false
```

### Pour Serveur PvE

```toml
allowPvP = false
respectClaims = true
pvpDamageMultiplier = 0.0
globalShadowLimit = 2000
```

### Pour Serveur PvP

```toml
allowPvP = true
pvpDamageMultiplier = 0.75
globalSummonCooldown = 60
perPlayerShadowLimit = 80
```

### Pour Roleplay

```toml
shadowsDropLoot = false
shadowXPMultiplier = 0.0
summonCost = 500
domainAccessCost = 100
```

### Pour Mode Hardcore/Difficult

```toml
ariseSuccessRate = 75
shadowStatsMultiplier = 0.8
ariseCooldown = 10
maxShadowSlots = 50
```

---

## 🔄 Commandes Admin

### Commandes In-Game

```
/shadowmonarch reload
  → Recharge la config sans redémarrer

/shadowmonarch debug <player>
  → Affiche debug info d'un joueur

/shadowmonarch clear <player>
  → Clear toutes les Ombres d'un joueur

/shadowmonarch give <player> <item> [amount]
  → Donne items du mod

/shadowmonarch setslots <player> <amount>
  → Modifie slots d'un joueur

/shadowmonarch ban <mob_id>
  → Ban un mob de conversion

/shadowmonarch unban <mob_id>
  → Unban un mob
```

---

## 🛡️ Permissions (Serveur)

### LuckPerms / PermissionsEx

```yaml
permissions:
  shadowmonarch.use: true          # Utiliser le mod
  shadowmonarch.arise: true        # Sort Arise
  shadowmonarch.domain: true       # Accès Domain
  shadowmonarch.army: true         # Invoquer armée
  shadowmonarch.pvp: true          # PvP avec Ombres
  shadowmonarch.admin: false       # Commandes admin
  shadowmonarch.bypass.cooldown: false  # Bypass cooldowns
  shadowmonarch.bypass.limit: false     # Bypass slot limits
```

### Groupes Recommandés

**Joueur Standard :**
```yaml
- shadowmonarch.use
- shadowmonarch.arise
- shadowmonarch.domain
- shadowmonarch.army
```

**VIP :**
```yaml
- shadowmonarch.*
- shadowmonarch.bypass.cooldown
```

**Admin :**
```yaml
- shadowmonarch.admin
- shadowmonarch.*
```

---

## 📊 Monitoring Serveur

### Métriques Importantes

**Via logs ou plugins:**

- Nombre total d'Ombres actives
- Ombres par joueur
- Lag causé par Ombres
- Crashes liés au mod

### Commande Debug

```
/shadowmonarch stats
```

**Output :**
```
=== Shadow Monarch Stats ===
Total Shadows: 487
Active Summoned: 124
Players with Shadows: 23
Average per Player: 21.2
Global Limit: 1000 (48.7% used)
TPS Impact: -0.3 (acceptable)
```

---

## 🔧 Troubleshooting Config

### Problème : Config ne se charge pas

**Solution :**
1. Vérifiez syntaxe TOML (pas d'erreurs)
2. Supprimez config et relancez (reset)
3. Utilisez validateur TOML en ligne

### Problème : Modifications ignorées

**Solution :**
1. Utilisez `/shadowmonarch reload`
2. Redémarrez complètement le serveur
3. Vérifiez qu'aucun plugin n'override

### Problème : mob_tiers.json cassé

**Solution :**
1. Validez JSON sur jsonlint.com
2. Restaurez backup par défaut
3. Ajoutez mobs un par un

---

## 💾 Sauvegardes

**Sauvegardez régulièrement :**

```
/config/shadowmonarch/  → Backup complet
/saves/[world]/shadowmonarch/  → Données joueurs
```

**Avant update du mod, faites backup !**

---

## 📖 Documentation API

Pour les développeurs souhaitant intégrer avec Shadow Monarch :

**JavaDocs :** [Lien vers docs](#)  
**Exemples :** [GitHub Wiki](https://github.com/votre-pseudo/shadow-monarch-mod/wiki/API)

---

## 🔗 Liens Utiles

- 📋 **Config par Défaut** : [GitHub](https://github.com/votre-pseudo/shadow-monarch-mod/tree/main/src/main/resources)
- 💬 **Aide Config** : [Discord #support](community/links.md)
- 🐛 **Bug Config** : [GitHub Issues](https://github.com/votre-pseudo/shadow-monarch-mod/issues)

---

!!! warning "Modifications Avancées"
    Modifiez seulement si vous savez ce que vous faites. Une mauvaise config peut casser le mod ou causer des crashes.

!!! tip "Backup First"
    Toujours faire un backup avant de modifier une config ! 💾