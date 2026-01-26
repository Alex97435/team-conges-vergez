# 🏥 TEAM Cabinet VERGEZ - Gestion des Congés

Application web de gestion des congés pour le Cabinet VERGEZ & Associés.

## ✨ Fonctionnalités

- **Tableau de bord** : Vue d'ensemble des congés par employé
- **Calendrier mensuel** : Visualisation des absences jour par jour
- **Import Excel** : Importation automatique du calendrier des absences
- **Règles métier** :
  - Maximum 3 semaines consécutives de congés par an
  - Aucun congé autorisé quand le Dr VERGEZ est présent
- **Solde automatique** : Calcul du solde de congés restant

## 🎨 Types d'absences

| Code | Type | Couleur |
|------|------|---------|
| C | Congé | Vert |
| SS | Sans solde | Orange |
| M | Maladie | Rouge |
| F | Formation | Violet |

## 🚀 Déploiement

### Vercel (recommandé)

1. Forkez ce repository sur GitHub
2. Connectez-vous à [Vercel](https://vercel.com)
3. Importez le projet depuis GitHub
4. Déployez !

### Local

```bash
# Cloner le repo
git clone https://github.com/votre-username/team-conges-vergez.git

# Aller dans le dossier
cd team-conges-vergez

# Lancer un serveur local
npx serve .
```

## 📁 Structure

```
team-conges-vergez/
├── index.html      # Application complète (React + styles)
├── package.json    # Configuration npm
├── vercel.json     # Configuration Vercel
└── README.md       # Documentation
```

## 📊 Import des données

L'application accepte les fichiers Excel (.xlsx) avec la structure suivante :
- Une feuille par mois (Janvier, Février, Mars, etc.)
- Colonnes : Nom de l'employé, puis jours 1 à 31
- Valeurs : C (Congé), SS (Sans solde), M (Maladie), F (Formation)

## 🔒 Stockage

Les données sont stockées localement dans le navigateur (localStorage).
Aucune donnée n'est envoyée à un serveur externe.

## 👨‍💻 Développé par

DBS360 - Digital Business Solutions

---

© 2025 Cabinet VERGEZ & Associés
