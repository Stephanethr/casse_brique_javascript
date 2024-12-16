# Projet : Jeu Casse-brique avec gestion des utilisateurs

Ce projet intègre un jeu de casse-brique développé en JavaScript dans une application Flask permettant la gestion des utilisateurs, l'enregistrement des scores, et la persistance des données à l'aide d'une base de données SQLite.

## Fonctionnalités principales

1. **Jeu Casse-brique :**
   - Jouez à un jeu interactif en HTML5 Canvas avec JavaScript.

2. **Gestion des utilisateurs :**
   - Inscription avec un nom d'utilisateur et un mot de passe.
   - Connexion sécurisée.
   - Déconnexion.

3. **Scores des joueurs :**
   - Enregistrement automatique du meilleur score du joueur.
   - Affichage du meilleur score de l'utilisateur sur l'interface du jeu.

## Structure du projet

```
project/
│
├── app.py                # Code principal de l'application Flask
├── templates/            # Fichiers HTML
│   ├── index.html        # Interface principale avec le jeu
│   ├── login.html        # Page de connexion
│   └── register.html     # Page d'inscription
├── static/               # Fichiers statiques (CSS, JS, etc.)
│   ├── style.css         # Styles CSS pour l'interface
│   └── app.js            # Logique JavaScript du jeu
└── game.db               # Base de données SQLite (générée automatiquement)
```

## Installation

### Prérequis
- **Python 3.7+**
- **Virtualenv** (recommandé)

### Étapes
1. Clonez le dépôt ou téléchargez les fichiers du projet :
   ```bash
   git clone https://github.com/Stephanethr/casse_brique_javascript
   cd casse_brique_javascript
   ```

2. Créez un environnement virtuel et activez-le :
   ```bash
   python -m venv env
   source env/bin/activate # Sur Windows : env\Scripts\activate
   ```

3. Installez les dépendances Python :
   ```bash
   pip install -r requirements.txt
   ```

4. Créer un fichier `.env` à la racine du projet avec les variables d'environnement suivantes :
   ```
    SECRET_KEY=your_secret_key
    ```
   
5. Lancez l'application Flask :
   ```bash
   python app.py
   ```

6. Accédez à l'application dans votre navigateur à l'adresse :
   ```
   http://127.0.0.1:5000
   ```

## Utilisation

1. **Inscription :**
   - Accédez à la page d'inscription pour créer un compte.

2. **Connexion :**
   - Connectez-vous avec vos identifiants pour accéder au jeu.

3. **Jouer :**
   - Jouez au casse-brique. Votre meilleur score sera automatiquement sauvegardé.

4. **Déconnexion :**
   - Cliquez sur le bouton "Déconnexion" pour quitter votre session.

## Développement

- **app.py** :
  - Gère les routes Flask pour l'inscription, la connexion, la mise à jour des scores, et le jeu.
  - Base de données SQLite avec SQLAlchemy pour stocker les utilisateurs et leurs scores.

- **HTML/CSS/JS** :
  - Interface utilisateur moderne avec des styles et interactions personnalisés.
  - Jeu interactif écrit en JavaScript avec logique de mise à jour des scores via une API Flask.

## Améliorations futures

- Ajouter des niveaux supplémentaires au jeu.
- Implémenter un classement global pour afficher les meilleurs scores de tous les joueurs.
- Ajouter des animations et sons pour améliorer l'expérience de jeu.

## Auteurs
- **Nom de l'auteur** - Développeur principal

## Licence
Ce projet est sous licence MIT. Consultez le fichier LICENSE pour plus d'informations.

