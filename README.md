# Ce que j'ai appris — Exercice API Testing avec Postman

## Exercice 2.1 — Envoi de données (POST)

J'ai appris à envoyer des données structurées via le Body d'une requête POST, en utilisant le format JSON dans l'onglet **Body → raw → JSON**. Exemple utilisé :

```json
{
  "prenom": "Donita",
  "objectif": "QA Analyst"
}
```

**Ce que ça m'a permis de comprendre :**
- Comment envoyer un payload JSON dans une requête HTTP
- Comment postman-echo.com me renvoie mes propres données dans le champ `json` de la réponse, ce qui permet de vérifier que ce qui a été envoyé correspond à ce qui a été reçu
- La différence entre les paramètres d'une requête GET (dans l'URL) et le contenu d'une requête POST (dans le Body)

## Exercice 2.2 — Variables d'environnement

J'ai créé un environnement Postman contenant une variable réutilisable :

Puis j'ai remplacé l'URL codée en dur par `{{base_url}}/get`.

**Compétence clé acquise : éviter le hardcoding**

C'est une compétence essentielle en QA parce que :
- Si l'URL de base change (ex: passage de dev à staging à prod), je n'ai qu'un seul endroit à modifier — la variable — plutôt que chaque requête individuellement
- Ça rend mes collections de tests réutilisables dans différents environnements
- C'est une pratique standard dans les vraies équipes QA en entreprise

## Résumé

| Concept | Compétence développée |
|---|---|
| Body → raw → JSON | Envoyer des données structurées dans une requête POST |
| Comparer input/output | Valider qu'une API traite correctement les données reçues |
| Variables d'environnement | Écrire des tests maintenables et réutilisables |
