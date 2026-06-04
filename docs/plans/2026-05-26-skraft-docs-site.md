# Plan — Alignement navigation `skraft-plugin` sur `learning-path-copilot`

**Date** : 2026-05-26  
**Objectif** : simplifier la navigation du site `skraft-plugin` en reprenant les principes visibles dans `learning-path-copilot` : peu d’entrées globales, progression guidée à gauche, et contenu centré sur l’essentiel.

---

## Exigences produit

1. **Aligner la navigation** avec la structure pédagogique du handbook.
2. **Réduire le nombre d’items de menu** global pour mettre en avant les contenus majeurs.
3. **Documenter chaque phase dans le menu de gauche** (ordre de lecture explicite).
4. **Expliquer les agents** : rôle, valeur, limites, cas d’usage.
5. **Rendre explicites les principes et les gates** qui gouvernent le workflow.
6. **Appuyer le discours avec des références externes** (ex. Martin Fowler) et créer une page dédiée quand un sujet mérite un chapitre complet.

---

## Proposition d’architecture de navigation

### Menu principal (minimal)

- Handbook
- Référence
- Méthodologie
- Ressources

Principe : pas de “mega-menu” orienté outils ; l’entrée principale reste le parcours.

### Menu gauche (phase-driven)

Dans la section Handbook, afficher les phases dans l’ordre :

1. Vision & cadrage
2. Design des agents
3. Rédaction assistée
4. Revue & gates qualité
5. Publication & amélioration continue

Chaque phase contient :
- le **pourquoi**,
- les **agents impliqués**,
- les **gates** d’entrée/sortie,
- les liens vers exemples et chapitres associés.

---

## Chapitres de fond à prévoir

- **Pourquoi un orchestrateur ?** (single entrypoint, gouvernance)
- **Principes de gates** (qualité, sécurité, traçabilité)
- **Pourquoi le reviewer doit être “fresh context”**
- **Boucle d’alignement bornée** (max rounds, escalade humaine)

Quand un sous-thème dépasse une section courte, créer un chapitre dédié plutôt qu’un paragraphe dense.

---

## Références d’autorité à citer

- Martin Fowler — écrits sur l’architecture évolutive et les pratiques de refactoring incrémental.
- Jez Humble & David Farley — principes de Continuous Delivery et quality gates.
- Gene Kim et al. — pratiques de flux et fiabilité opérationnelle.

Ces références servent de cadre, pas d’argument d’autorité isolé : chaque citation doit être reliée à une décision concrète de navigation ou de workflow.

---

## Critères d’acceptation

- Navigation globale raccourcie et compréhensible en < 10 secondes.
- Parcours gauche structuré par phases, sans ambiguïté d’ordre.
- Chaque phase explique agents + principes + gates.
- Les chapitres avancés existent pour les sujets complexes.
- Les pages mentionnent des références reconnues et contextualisées.
