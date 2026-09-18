# Lab 001 — SQL injection

**Plateforme :** PortSwigger Web Security Academy

## Objectif

Afficher les produits masqués en contournant le filtre de catégorie.

## Étapes

1. Ouvrir une catégorie de produits.
2. Modifier le paramètre `category`.
3. Utiliser :

```text
' OR 1=1 --
```

## Résultat

Les produits d'autres catégories sont affichés et le lab est validé.

![Page initiale](01-storefront.png)

![Catégorie filtrée](02-filtered-category.png)

![Lab résolu](03-sql-injection-success.png)

> Lab PortSwigger réalisé dans un environnement autorisé.
