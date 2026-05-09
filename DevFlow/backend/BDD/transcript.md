# Transcript — Réunion Client / Équipe Backend
## Projet : DevFlow
## Sujet : Kickoff Technique & Définition Architecture Backend

**Participants**
- Emma — Product Manager
- Lukas — Lead Backend Engineer
- Sofia — DevOps Engineer
- Martin — CTO
- Vous — Backend Engineer Consultant

---

# Début de réunion

## Emma (Product Manager)

Bonjour à tous.

L’objectif de cette réunion est d’aligner les équipes sur le périmètre du projet DevFlow et de commencer à définir les choix techniques backend.

Comme vous le savez, nous voulons construire une plateforme interne de gestion de projets techniques capable de remplacer plusieurs outils actuellement utilisés séparément.

Nous avons besoin d’une base backend solide et scalable.

---

# Présentation du besoin métier

## Emma

Aujourd’hui, nos équipes utilisent :
- Jira
- Slack
- des fichiers Excel
- des outils internes

Cela crée :
- des pertes d’informations
- des problèmes de synchronisation
- des difficultés de suivi projet

Nous voulons centraliser :
- les projets
- les tickets
- les workflows
- les notifications

---

# Discussion architecture

## Lukas (Lead Backend Engineer)

D’un point de vue technique, nous voulons partir sur une architecture modulaire avec NestJS.

L’idée est d’avoir :
- une API REST propre
- des modules indépendants
- une architecture maintenable

Nous voulons éviter un monolithe mal structuré.

---

## Vous

D’accord.

Est-ce que vous avez déjà défini les principaux domaines métier du backend ?

---

## Lukas

Oui, globalement nous aurons :

```txt
auth
users
projects
tickets
comments
notifications