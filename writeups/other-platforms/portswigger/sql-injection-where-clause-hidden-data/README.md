# SQL injection in WHERE clause allowing retrieval of hidden data

**Plateforme :** PortSwigger Web Security Academy
**Type :** SQL injection
**Difficulté :** Apprentice

## Objectif

Afficher les produits masqués en contournant le filtre de catégorie.

## Étapes

1. Ouvrir une catégorie de produits.
2. Tester le paramètre `category` dans l'URL.
3. Ajouter la charge utile suivante :

```text
' OR 1=1 --
```

## Résultat

Le filtre est contourné et les produits d'autres catégories s'affichent.

![Lab résolu](assets/03-sql-injection-success.png)

## Correction

- Utiliser des requêtes paramétrées.
- Valider les entrées côté serveur.

> Lab réalisé uniquement dans l'environnement PortSwigger autorisé.
