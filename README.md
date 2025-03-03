# GESTION DES TACHES

**GESTION DES TACHES** est une application CRUD (Create, Read, Update, Delete) simple construite avec **FASTAPI**. Cette application permet aux utilisateurs de gérer leurs tâches efficacement.

## Fonctionnalités

- Créer de nouvelles tâches
- Lire les tâches existantes
- Mettre à jour les détails d'une tâche
- Supprimer des tâches

## Installation

1. **Cloner le dépôt :**

   ```bash
   git clone https://github.com/yourusername/gestion-des-taches.git
   cd gestion-des-taches
   ```

2. **Créer et activer un environnement virtuel :**

   ```bash
   python -m venv venv
   source venv/bin/activate  # Sur Windows utilisez `venv\Scripts\activate`
   ```

3. **Installer les dépendances requises :**

   ```bash
   pip install -r requirements.txt
   ```

4. **Lancer l'application :**

   ```bash
   uvicorn main:app --reload
   ```

   L'application sera disponible à [http://127.0.0.1:8000](http://127.0.0.1:8000).

## Utilisation

### Créer une nouvelle tâche :

**Requête :**
```http
POST /tasks/
```
**Exemple de corps de requête :**
```json
{
  "title": "Titre de la tâche",
  "description": "Description de la tâche",
  "completed": false
}
```

### Lire toutes les tâches :

```http
GET /tasks/
```

### Lire une tâche spécifique :

```http
GET /tasks/{task_id}
```

### Mettre à jour une tâche :

**Requête :**
```http
PUT /tasks/{task_id}
```
**Exemple de corps de requête :**
```json
{
  "title": "Titre mis à jour",
  "description": "Description mise à jour",
  "completed": true
}
```

### Supprimer une tâche :

```http
DELETE /tasks/{task_id}
```

## Contribution

Les contributions sont les bienvenues ! Merci d'ouvrir une issue ou de soumettre une pull request.

## Licence

Ce projet est sous licence **MIT**. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## Contact

Si vous avez des questions ou des suggestions, n'hésitez pas à me contacter : **[omarbouhdiida@gmail.com](mailto:omarbouhdiida@gmail.com)**

