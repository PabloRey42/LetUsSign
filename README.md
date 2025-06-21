# LetUsSign

Plateforme nationale de gestion d'établissement scolaire. Cette application
propose une interface web (React.js) et mobile (React Native) communiquant avec
une API Django REST. Elle permet la gestion des utilisateurs (élèves, parents,
enseignants, administrateurs), la consultation des emplois du temps et des
notes, ainsi que la signature électronique des documents via l'API Universign.

## Fonctionnalités prévues

- Authentification par JWT ou OAuth2
- Gestion des rôles et permissions
- Suivi des élèves, classes et matières
- Emplois du temps et notes
- Signature électronique certifiée eIDAS/RGS
- Notifications temps réel (Firebase Cloud Messaging)

## Arborescence du dépôt

```
backend/    # Projet Django + API REST
frontend/   # Application React (placeholder)
mobile/     # Application React Native (placeholder)
```

## Démarrage rapide (back‑end)

1. Installez Python 3.12 et PostgreSQL.
2. Créez un environnement virtuel puis installez les dépendances :
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   pip install -r backend/requirements.txt
   ```
3. Configurez les variables d'environnement dans `.env` ou via l'OS
   (voir `backend/config/settings.py`).
4. Exécutez les migrations et lancez le serveur :
   ```bash
   python backend/manage.py migrate
   python backend/manage.py runserver
   ```

## Test unitaire

Aucun test n'est fourni pour l'instant. Ajoutez vos tests avec `pytest` ou
`python manage.py test`.

## Frontend et mobile

Les dossiers `frontend` et `mobile` sont vides pour le moment. Ils accueilleront
respectivement l'application React et l'application React Native.
