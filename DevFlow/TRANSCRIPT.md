# Transcript Client — Projet Backend "DevFlow"

## Contexte

Le client est une entreprise technologique en croissance qui gère plusieurs équipes de développement logiciel réparties entre différents pays européens.

Les équipes utilisent actuellement plusieurs outils séparés :
- gestion de tickets
- suivi de projet
- documentation
- notifications

Le client souhaite centraliser ces fonctionnalités dans une plateforme backend moderne, scalable et sécurisée.

---

# Transcript — Kickoff Meeting

## Client

Bonjour,

Nous recherchons un backend engineer capable de développer le socle technique d’une plateforme interne de gestion de projets techniques.

Aujourd’hui, nos équipes utilisent différents outils et nous avons plusieurs problèmes :
- manque de centralisation
- difficultés de suivi des tickets
- faible visibilité sur l’avancement des projets
- notifications peu fiables
- problèmes de performance sur certains workflows

Nous souhaitons construire une solution backend moderne capable de supporter notre croissance.

---

# Objectifs métier

## 1. Gestion centralisée des projets

Chaque équipe doit pouvoir :
- créer des projets
- inviter des collaborateurs
- gérer les permissions
- suivre les tâches associées

---

## 2. Gestion des tickets techniques

Nous avons besoin :
- d’un système de tickets
- d’un workflow configurable
- d’une gestion des priorités
- d’une assignation des tâches

Exemple de statuts :
- TODO
- IN_PROGRESS
- REVIEW
- DONE

---

## 3. Authentification & sécurité

Le système doit inclure :
- authentification sécurisée
- gestion des rôles
- permissions utilisateurs
- protection API

Nous souhaitons utiliser JWT pour l’authentification.

---

## 4. Performance & scalabilité

La plateforme doit pouvoir :
- gérer plusieurs équipes simultanément
- supporter une montée en charge progressive
- rester maintenable dans le temps

Nous voulons une architecture modulaire et scalable.

---

## 5. API Backend

Nous voulons une API REST claire et documentée permettant :
- création/modification de tickets
- gestion utilisateurs
- notifications
- suivi activité

La documentation Swagger est fortement souhaitée.

---

# Contraintes techniques

## Backend

Technologies souhaitées :
- TypeScript
- Node.js
- NestJS

---

## Base de données

Technologies souhaitées :
- PostgreSQL

Nous voulons une structure relationnelle propre et maintenable.

---

## Infrastructure

L’application doit être :
- dockerisée
- facilement déployable
- compatible CI/CD

---

## Sécurité

Nous attendons :
- validation des données
- protection contre les abus API
- gestion des permissions
- hash des mots de passe

---

# Fonctionnalités MVP

## Utilisateurs
- inscription
- connexion
- refresh token
- rôles utilisateurs

---

## Projets
- création projet
- suppression projet
- ajout membres
- permissions

---

## Tickets
- création ticket
- modification ticket
- assignation
- priorité
- deadline
- commentaires

---

## Notifications
- notification lors d’assignation
- notification changement de statut

---

# Fonctionnalités avancées (bonus)

## Temps réel
Support WebSockets pour :
- notifications live
- mise à jour temps réel

---

## Cache
Utilisation Redis pour :
- optimisation performances
- gestion sessions

---

## Queue System
Support des tâches asynchrones :
- emails
- notifications
- traitements lourds

---

# Exigences qualité

Le code doit être :
- propre
- documenté
- maintenable
- modulaire

Nous attendons :
- architecture claire
- séparation des responsabilités
- bonnes pratiques backend modernes

---

# Architecture attendue

```txt
src/
 ├── auth/
 ├── users/
 ├── projects/
 ├── tickets/
 ├── comments/
 ├── notifications/
 ├── common/