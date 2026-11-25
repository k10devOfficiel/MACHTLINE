# Rendez-vous

Jeu web de simulation sociale 18+ en temps réel.

## Prérequis

- [Node.js](https://nodejs.org/) (v20 ou plus récent)
- npm
- PostgreSQL (pour les prochaines étapes)

## Installation

1. Cloner le dépôt puis installer les dépendances du serveur :
   ```bash
   cd server
   npm install
   ```

2. Créer le fichier d'environnement du serveur à partir de l'exemple :
   ```bash
   cp .env.example .env
   ```
   *(Sur Windows PowerShell : `Copy-Item .env.example .env`)*

3. Installer les dépendances du client :
   ```bash
   cd ../client
   npm install
   ```

## Lancer le projet en développement

Ouvre **deux terminaux** :

- **Terminal 1 (Serveur)** :
  ```bash
  cd server
  npm run dev
  ```
  Le serveur écoute sur `http://localhost:3000`.
  Vérification : `http://localhost:3000/api/health` doit renvoyer `{"status":"ok"}`.

- **Terminal 2 (Client)** :
  ```bash
  cd client
  npm run dev
  ```
  Le client est accessible sur `http://localhost:5173`.
