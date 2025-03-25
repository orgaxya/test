**Document de Spécification du Produit (PRD) : Journal des Transactions**

## 1. Contexte et Problématique

Dans le cadre de l'amélioration de la transparence et de la conformité financière, les organisations doivent maintenir un journal des dépenses et des revenus associés à un projet. Afin de structurer ces données de manière rigoureuse, nous allons implémenter un journal des transactions en suivant le modèle de comptabilité en partie double (transaction log pattern).

## 2. Objectifs

L'objectif est de développer un système permettant de suivre toutes les transactions (entrées et sorties de fonds) associées à un projet. Ce journal devra être affiché sous forme de tableau et permettre les opérations CRUD de base : création, lecture, mise à jour et suppression des transactions.

## 3. Spécifications Fonctionnelles

### 3.1. Affichage du Journal des Transactions

Le journal des transactions devra être présenté sous forme de tableau avec les colonnes suivantes :

- **Date** : Date de la transaction
- **Notes** : Description de la transaction
- **Débit** : Montant débité (sortie de fonds)
- **Crédit** : Montant crédité (entrée de fonds)
- **Total** : Solde actuel après la transaction

### 3.2. Fonctionnalités

- **Création** : Ajouter une nouvelle transaction (débit ou crédit) avec une description.
- **Lecture** : Afficher la liste des transactions dans un tableau interactif.
- **Mise à jour** : Modifier les détails d'une transaction existante.
- **Suppression** : Supprimer une transaction.

### 3.3. Expérience Utilisateur (UX/UI)

- Interface ergonomique et intuitive
- Utilisation de composants UI modernes et cohérents
- Gestion fluide des interactions (ajout, modification, suppression)
- Affichage adaptatif (responsive design)

## 4. Critères de Test et de Validation

Les tests porteront sur les critères suivants :

- **Précision et rigueur** : Les transactions doivent être correctement enregistrées et affichées.
- **Expérience utilisateur** : Navigation fluide et interface claire.
- **Code réutilisable et bien structuré** : Bonnes pratiques de développement et conception technique bien pensée.

## 5. Technologies Utilisées

- **Framework Frontend & Backend** : Next.js avec App Router
- **Gestion des API** : tRPC
- **Base de données** : MySQL via Drizzle ORM
- **Stack de développement** : T3 Stack (Next.js + tRPC + Drizzle)
- **Interface utilisateur** : shadcn et data-table

## 6. Scénario d'Utilisation

**Hypothèse de départ** : L'utilisateur gère un budget initial de 1000 \$.

1. Il ajoute une transaction de 200 \$ de débit avec la note "Achat de matériaux".
2. Il ajoute une transaction de 500 \$ de crédit avec la note "Subvention reçue".
3. Il met à jour la transaction de 200 \$ pour corriger le montant à 250 \$.
4. Il consulte l'historique des transactions et vérifie le solde.
5. Il supprime une transaction et vérifie l'actualisation du solde.

## 7. Livrables Attendus

- Une interface plaisante à l'œil avec une bonne expérience utilisateur.
- Un screenshot montrant l'implémentation de l'interface utilisateur.
- Un lien Github avec un README expliquant les choix techniques et l'implémentation.

**Note :** L'authentification n'est pas requise pour ce test.
