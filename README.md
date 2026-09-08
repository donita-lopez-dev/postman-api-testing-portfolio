# API Testing review

Tests API réalisés avec Postman dans le cadre de ma formation QA.

## Structure du projet

- **Collection** : contient les requêtes API (GET, POST) ainsi que leurs paramètres et scripts de test
- **Environnement** : contient les variables réutilisables (ex. `base_url`) utilisées dans les requêtes de la collection

## Endpoints testés
- GET/POST sur postman-echo.com
- Validation status code, temps de réponse, structure JSON

## Environnements
- `dev.postman_environment.json` — variables de base (`base_url`)

## Comment utiliser
1. Importer `My-Collection.postman_collection.json` dans Postman
2. Importer `dev.postman_environment.json` et le sélectionner comme environnement actif
3. Lancer via Collection Runner
