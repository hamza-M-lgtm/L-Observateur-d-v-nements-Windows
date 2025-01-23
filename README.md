# L-Observateur-d-v-nements-Windows
## Challenge : Configuration de ta vue personnalisée

### 2. Installer le rôle DNS
- Ouvrez le `Gestionnaire de serveur`.
- Cliquez sur `Ajouter des rôles et des fonctionnalités`.
- Sélectionnez le `Serveur DNS` et suivez les étapes pour l'installer.
- ![Image](https://github.com/user-attachments/assets/2ffa0d48-d3cc-416c-9b2f-35dd1afe1603)

### 3. Créer une vue personnalisée dans l'Event Viewer
- Ouvrez l'`Observateur d'événements` (`eventvwr`).

- ![Image](https://github.com/user-attachments/assets/fd07b28d-38b9-4aa4-8320-e1fa800ff29a)
  
- Cliquez droit sur `Vues personnalisées` et sélectionnez `Créer une vue personnalisée`.

### 4. Configurer les filtres de la vue personnalisée
- **Niveaux à surveiller** : Cochez `Critique`, `Erreur`, `Avertissement` et `Information`.
- **Sources d'événements** : Cochez `DNS-Server-Service` et `DNS Client Events`.
- **ID d'événement** : Dans le champ `Tous les ID d'événements`, entrez les ID suivants séparés par des virgules : `2, 4, 409, 501, 502, 6001, 6002`.

![Image](https://github.com/user-attachments/assets/2f413f61-6801-41d7-98b0-ef08f317792b)

### 5. Nommer et enregistrer la vue personnalisée

- Donnez un nom clair et descriptif à la vue personnalisée, par exemple : `Surveillance DNS`.
- Cliquez sur `OK` pour enregistrer.
- ![Image](https://github.com/user-attachments/assets/5a999c80-f411-4274-b542-0e729df67f16)

### 6. Exporter la vue au format XML
- Cliquez droit sur la vue personnalisée nouvellement créée et sélectionnez `Exporter la vue...`.
- Enregistrez le fichier XML.
- ![Image](https://github.com/user-attachments/assets/718c170c-d6f3-4261-8537-9717fb61abc4)

