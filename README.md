Task Manager
Description
Task Manager est une application web permettant de gérer des tâches. Elle est composée de deux parties principales :

Backend : Un serveur Express avec une base de données PostgreSQL pour gérer les tâches.
Frontend : Une interface utilisateur React pour interagir avec le backend.
Prérequis
Avant de commencer, assurez-vous d'avoir installé les outils suivants :

Node.js (version 14 ou supérieure)
npm ou Yarn
PostgreSQL (pour la base de données)
Installation
1. Cloner le dépôt
bash
Copier le code
git clone https://github.com/votre-utilisateur/task-manager.git
cd task-manager
2. Configuration du Backend
Accédez au répertoire backend :

bash
Copier le code
cd backend
Installez les dépendances :

bash
Copier le code
npm install
Créez un fichier .env à la racine du répertoire backend et ajoutez les variables d'environnement suivantes :

env
Copier le code
DB_NAME=nom_de_votre_base_de_données
DB_USER=nom_utilisateur
DB_PASSWORD=mot_de_passe
DB_HOST=localhost
JWT_SECRET=votre_clé_secrète
PORT=5001
Démarrez le serveur backend :

bash
Copier le code
npm start
3. Configuration du Frontend
Accédez au répertoire frontend :

bash
Copier le code
cd ../frontend
Installez les dépendances :

bash
Copier le code
npm install
Créez un fichier .env à la racine du répertoire frontend et ajoutez les variables d'environnement suivantes :

env
Copier le code
REACT_APP_API_URL=http://localhost:5001
Démarrez l'application frontend :

bash
Copier le code
npm start
Utilisation
Backend : Le serveur backend est accessible à http://localhost:5001. Il gère les requêtes API pour les tâches.
Frontend : L'application frontend est accessible à http://localhost:3000. Vous pouvez ajouter, modifier, supprimer et afficher des tâches via l'interface utilisateur.
Endpoints API
GET /api/tasks : Récupère toutes les tâches.
POST /api/tasks : Crée une nouvelle tâche.
PUT /api/tasks/
: Met à jour une tâche existante.
DELETE /api/tasks/
: Supprime une tâche.
Notes
Assurez-vous que les ports configurés dans le backend et le frontend sont cohérents.
Pour les environnements de production, vous devrez ajuster les configurations de sécurité et CORS.
Contribution
Les contributions sont les bienvenues ! Veuillez soumettre des pull requests pour les corrections de bogues ou les améliorations de fonctionnalités.

Licence
Ce projet est sous la licence MIT. Voir le fichier LICENSE pour plus d'informations.
