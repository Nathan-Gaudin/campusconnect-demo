# CampusConnect

> Plateforme permettant aux étudiants de découvrir les événements universitaires et de s'y inscrire.
> Projet Scrum du **Groupe Phonk** (projet Jira **CCG2**).

## ⚠️ État réel du projet : conception

CampusConnect est **en phase de conception**. Ce dépôt est **documentaire** : il ne contient **aucun code applicatif**, aucune procédure d'installation et aucun pipeline CI/CD.
Les fonctionnalités listées ci-dessous sont **envisagées** et ne sont **pas développées**. Les avancements visibles dans Jira pendant le Sprint 1 sont des simulations pédagogiques.

## Présentation et objectifs

CampusConnect doit centraliser la vie du campus en un seul endroit :

- permettre à un **étudiant** de trouver rapidement un événement qui l'intéresse et de réserver sa place ;
- permettre à un **organisateur** (association, administration) de publier un événement et de connaître les inscrits.

**Sprint Goal du Sprint 1** : permettre à un étudiant de découvrir les événements du campus publiés par un organisateur, de les retrouver facilement et de s'y inscrire — première livraison utilisable de CampusConnect.

## Fonctionnalités envisagées

| Fonctionnalité | User Story | Clé Jira | Priorité | Statut |
|---|---|---|---|---|
| Consulter la liste des événements à venir | US01 | CCG2-5 | Must | Prévue — Sprint 1 |
| Rechercher un événement (mot-clé, filtre) | US02 | CCG2-7 | Should | Prévue — Sprint 1 |
| S'inscrire à un événement | US03 | CCG2-6 | Must | Prévue — Sprint 1 |
| Annuler son inscription | US04 | CCG2-10 | Should | Product Backlog |
| Recevoir une notification | US05 | CCG2-11 | Could | Product Backlog (à découper) |
| Créer et publier un événement | US06 | CCG2-4 | Must | Prévue — Sprint 1 |
| Modifier un événement | US07 | CCG2-9 | Could | Product Backlog |
| Consulter la liste des inscrits | US08 | CCG2-8 | Should | Product Backlog |

« Prévue » signifie planifiée, **pas** réalisée.

## Outils

| Outil | Usage |
|---|---|
| **Jira** | Product Backlog, Sprints, suivi des User Stories — [Backlog CCG2](https://efrei-team-wowz5nfw.atlassian.net/jira/software/projects/CCG2/boards/34/backlog) |
| **Confluence** | Documentation fonctionnelle et technique — espace *Campus connect G2* |
| **GitHub** | Versionnement de la documentation (ce dépôt) et traçabilité avec Jira |
| **PlantUML** | Diagrammes UML (sources dans [`docs/uml`](docs/uml)) |

## Documentation

### Confluence

- [01 — Présentation du projet](https://efrei-team-wowz5nfw.atlassian.net/wiki/spaces/~712020ee249373bef849e0b7a15ede97def058/pages/14123010)
- [02 — Documentation fonctionnelle](https://efrei-team-wowz5nfw.atlassian.net/wiki/spaces/~712020ee249373bef849e0b7a15ede97def058/pages/14155777)
  - [Spécification fonctionnelle — US03 S'inscrire à un événement (CCG2-6)](https://efrei-team-wowz5nfw.atlassian.net/wiki/spaces/~712020ee249373bef849e0b7a15ede97def058/pages/14188545)
- [03 — Documentation technique (diagrammes UML)](https://efrei-team-wowz5nfw.atlassian.net/wiki/spaces/~712020ee249373bef849e0b7a15ede97def058/pages/14155824)
- [04 — Gestion Agile](https://efrei-team-wowz5nfw.atlassian.net/wiki/spaces/~712020ee249373bef849e0b7a15ede97def058/pages/14254087)
- [05 — Guide utilisateur](https://efrei-team-wowz5nfw.atlassian.net/wiki/spaces/~712020ee249373bef849e0b7a15ede97def058/pages/14221319)

L'espace Confluence est réservé aux membres de l'équipe : une connexion au site Atlassian est nécessaire.

### Diagrammes UML (sources modifiables)

| Diagramme | Source |
|---|---|
| Cas d'utilisation | [`docs/uml/cas-utilisation.puml`](docs/uml/cas-utilisation.puml) |
| Classes (Etudiant, Evenement, Inscription…) | [`docs/uml/classes.puml`](docs/uml/classes.puml) |
| Séquence — inscription à un événement | [`docs/uml/sequence-inscription.puml`](docs/uml/sequence-inscription.puml) |

Les images générées sont intégrées dans la page Confluence *03 — Documentation technique*.

### Autres fichiers

- `SPRINT_NOTES.md` — Sprint Goal et compte rendu de planification du Sprint 1, proposé dans la [PR #1](https://github.com/Nathan-Gaudin/campusconnect-demo/pull/1) (branche `docs/CCG2-5-sprint-notes`, CCG2-5).

## Consignes de contribution

1. **Partir d'un ticket Jira** : toute modification est liée à une clé `CCG2-x`.
2. **Créer une branche** nommée `type/CCG2-x-description`, par exemple `docs/CCG2-6-spec-inscription`.
3. **Mentionner la clé Jira** au début de chaque message de commit : `CCG2-6 docs: précise le scénario « événement complet »`.
4. **Ouvrir une Pull Request** avec la clé dans le titre et faire relire par au moins un autre membre avant fusion.
5. **Diagrammes** : modifier le fichier `.puml`, régénérer l'image et mettre à jour la page Confluence correspondante.
6. **Rester factuel** : ne pas présenter une fonctionnalité comme développée ou testée tant qu'elle ne l'est pas ; distinguer les règles validées par le Product Owner de celles qui restent à confirmer.
7. Ne publier **aucune donnée personnelle ou confidentielle** dans le dépôt.

## Équipe

| Membre | Responsabilités au Sprint 1 |
|---|---|
| Nathan Gaudin | US01 (CCG2-5), US02 (CCG2-7) |
| Noé de Rosny | US06 (CCG2-4) |
| Fatih Emiral | US03 (CCG2-6) |
