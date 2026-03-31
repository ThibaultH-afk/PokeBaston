# ⚡ PokeBaston

## 📋 Présentation du projet
**PokeBaston** est une application web simulant un duel entre deux dresseurs Pokémon. Ce projet universitaire est réalisé par une équipe de **5 étudiants**.

---

## 🔗 Liens Utiles

- **[INSTALLATION](docs/INSTALLATION.md)** - Instructions détaillées sur l'installation
- **[USER STORIES](docs/USERSTORIES.md)** - Description des User Stories
- **[CONVENTION COMMITS](docs/CONVENTION.md)** - Notre convention de commits utilisé
---

## 🎮 Contexte du jeu
Chaque dresseur doit choisir jusqu'à **6 Pokémon** parmi les 151 présents dans la première génération.

### Déroulement du combat
À l'issue de ce choix, les joueurs envoient un Pokémon chacun dans l'arène. Le premier joueur qui n'a plus de Pokémon a perdu le match.

* **Ordre d'attaque :** Le Pokémon avec la statistique de **vitesse** la plus élevée (en respectant les règles de priorité) commence.
* **Système de jeu :** Le combat se déroule au tour par tour. 
* **Interface :** Un message texte informe les deux joueurs de chaque action réalisée.

### Actions possibles (1 seule par tour)
| Action | Détails |
| :--- | :--- |
| **Changer de Pokémon** | Impossible de choisir un Pokémon qui n'a plus de PV. |
| **Attaquer** | La notion d'**efficacité des types** est prise en compte (ex: Eau > Feu). |

---

## 📊 Caractéristiques techniques

### Définition d'un Pokémon
Un Pokémon se définit par les statistiques suivantes :
* ❤️ **Points de vie (PV)**
* ⚔️ **Attaque** / 🛡️ **Défense**
* ✨ **Attaque Spéciale** / 🌀 **Défense Spéciale**
* ⚡ **Vitesse**

### Définition d'une attaque
Chaque capacité possède :
* **Puissance de base**
* **Type** (Élémentaire)
* **Catégorie** (Physique ou Spéciale)
* **Utilisations** (Nombre de PP)
