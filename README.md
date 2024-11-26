# **HireTrack**  
_**Repérez les opportunités qui façonnent votre avenir.**_

## **Description**
**HireTrack** est une application web moderne qui aide les utilisateurs à suivre et à découvrir des opportunités d'emploi correspondant à leurs préférences en temps réel. Grâce à une intégration avec l'API LinkedIn, l'application offre une interface intuitive pour rechercher, filtrer, et recevoir des notifications sur les nouvelles offres d'emploi.

---

## **Fonctionnalités**
### **Utilisateur**
- **Connexion via LinkedIn** : Authentifiez-vous facilement pour synchroniser votre profil LinkedIn.
- **Recherche d'opportunités** : Trouvez des offres d'emploi basées sur vos mots-clés et préférences.
- **Filtres dynamiques** : Affinez votre recherche par localisation, secteur, ou entreprise.
- **Notifications en temps réel** : Soyez informé des nouvelles opportunités via des notifications push.
- **Gestion de profil** : Enregistrez vos mots-clés et paramètres de recherche pour une expérience personnalisée.

### **Administrateur**
- **Suivi des utilisateurs actifs**.
- **Gestion des quotas d’appels API LinkedIn**.

---

## **Stack Technologique**
| **Catégorie**          | **Technologie**                      |
|-------------------------|--------------------------------------|
| **Frontend**            | React.js, Tailwind CSS, Axios       |
| **Backend**             | NestJS (Node.js), TypeScript        |
| **Base de Données**     | MongoDB (Mongoose)                  |
| **Notifications**       | Firebase Cloud Messaging            |
| **API et Intégration**  | LinkedIn API (OAuth 2.0, Jobs API)  |
| **Hébergement**         | Vercel (Frontend), AWS/Heroku (Backend) |
| **Gestion du Code**     | GitHub                              |

---

## **Prérequis**
### Outils nécessaires :
1. **Node.js** (v16+ recommandé)
2. **Yarn** (gestionnaire de paquets)
3. **MongoDB** (local ou Atlas)
4. **Compte Firebase** (pour les notifications push)
5. **Clés API LinkedIn** (OAuth 2.0 pour l’authentification)
6. **Git** pour la gestion du code source

---

## **Installation et Configuration**
### **Étape 1 : Cloner le dépôt**
```bash
git clone https://github.com/smartdev-ci/HireTrack.git
cd jobrader
```

### **Étape 2 : Configuration du Frontend**
1. Accédez au dossier `front-app` :
   ```bash
   cd front-app
   ```
2. Installez les dépendances :
   ```bash
   yarn install
   ```
3. Configurez les variables d’environnement dans un fichier `.env` :
   ```plaintext
   REACT_APP_API_BASE_URL=http://localhost:8200/api
   REACT_APP_FIREBASE_API_KEY=your_firebase_api_key
   ```
4. Lancez le serveur de développement :
   ```bash
   yarn start
   ```

---

### **Étape 3 : Configuration du Backend**
1. Accédez au dossier `back-app` :
   ```bash
   cd back-app
   ```
2. Installez les dépendances :
   ```bash
   yarn install
   ```
3. Configurez les variables d’environnement dans un fichier `.env` :
   ```plaintext
   MONGO_URI=your_mongodb_connection_string
   LINKEDIN_CLIENT_ID=your_linkedin_client_id
   LINKEDIN_CLIENT_SECRET=your_linkedin_client_secret
   FIREBASE_SERVER_KEY=your_firebase_server_key
   PORT=8200
   ```
4. Lancez le serveur backend :
   ```bash
   yarn start:dev
   ```

---

## **Utilisation**
1. Ouvrez l'application frontend sur `http://localhost:3000`.
2. Connectez-vous via LinkedIn.
3. Configurez vos préférences et recevez des notifications sur les nouvelles opportunités d'emploi.

---

## **Structure du Projet**
```
jobrader/
├── frontend/           # Application React.js
│   ├── src/
│   │   ├── components/ # Composants React
│   │   ├── pages/      # Pages principales
│   │   ├── hooks/      # Hooks personnalisés
│   │   └── styles/     # Fichiers CSS (Tailwind)
│   ├── public/
│   └── package.json
├── backend/            # Application NestJS
│   ├── src/
│   │   ├── modules/    # Modules NestJS (opportunities, users)
│   │   ├── controllers/ # Contrôleurs pour les endpoints API
│   │   └── services/   # Services métier
│   ├── test/           # Tests unitaires
│   └── package.json
└── README.md           # Documentation du projet
```

---

## **Roadmap**
1. **Phase 1** : Configuration initiale et intégration de l’API LinkedIn.
2. **Phase 2** : Développement du tableau de bord utilisateur et des filtres dynamiques.
3. **Phase 3** : Notifications en temps réel via Firebase.
4. **Phase 4** : Optimisation de l’application pour les performances et la scalabilité.
5. **Phase 5** : Tests finaux et déploiement.

---

## **Contribuer**
1. Forkez le projet.
2. Créez une branche pour votre fonctionnalité :
   ```bash
   git checkout -b feature/your-feature
   ```
3. Faites vos modifications et committez-les :
   ```bash
   git commit -m "Ajout d'une nouvelle fonctionnalité"
   ```
4. Envoyez votre branche vers le dépôt distant :
   ```bash
   git push origin feature/your-feature
   ```
5. Créez une pull request sur GitHub.

---

## **Licence**
Ce projet est sous licence MIT. Consultez le fichier [LICENSE](LICENSE) pour plus d'informations.
```

---
