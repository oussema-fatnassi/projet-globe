# Projet Globe

Refonte de l'intranet pédagogique de La Plateforme : un espace étudiant et un espace équipe pédagogique, accessibles par Google SSO.

Projet M1 (La Plateforme, Marseille 2026). Dans la posture d'un directeur technique, nous ne livrons pas de code : nous livrons la compréhension du besoin et la documentation qui permettra à une équipe de construire Globe et de le faire évoluer.

**Équipe :** Thanh Lemelle · Oussema Fatnassi

## Product Goal

D'ici le 1er janvier 2027, centraliser au moins 70 % des fonctionnalités aujourd'hui dispersées entre les outils de La Plateforme, dans un intranet unique accessible par Google SSO.

## Livrables demandés


| Fichier                                                                   | Contenu                                                                |
| ------------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| `[organigramme.pdf](organigramme.pdf)`                                    | Organigramme de l'équipe et rôles associés                             |
| `[cr_choix_methode.pdf](cr_choix_methode.pdf)`                            | Choix de Scrum, méthodes écartées et raisons                           |
| `[cahier_des_charges.pdf](cahier_des_charges.pdf)`                        | Exigences fonctionnelles (EF-01 à EF-15), contraintes, matrice d'accès |
| `[database_scheme.pdf](database_scheme.pdf)`                              | Modèle de données : MCD, MLD, MPD (PostgreSQL)                         |
| `[application_diagram.pdf](application_diagram.pdf)`                      | Diagramme de classes                                                   |
| `[onboarding.pptx](onboarding.pptx)` · `[onboarding.pdf](onboarding.pdf)` | Présentation d'accueil du nouveau développeur                          |




## Documents complémentaires


| Fichier                                                                    | Contenu                                                                       |
| -------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `[dossier_architecture_technique.pdf](dossier_architecture_technique.pdf)` | DAT : architecture, sécurité, RGPD, accessibilité, plan de tests, maintenance |
| `[cahier_de_recettes.pdf](cahier_de_recettes.pdf)`                         | Scénarios de recette (Sprint 1 : connexion Google, REC-AUTH-01 à 08)          |
| `[product_goal.pdf](product_goal.pdf)`                                     | Product Goal Canvas : objectif, vision, mesures, risques et équipe Scrum      |


Le planning (story map en 4 versions, Sprint 1 détaillé) et le backlog sont tenus dans Lucid et Jira (voir ci-dessous).

## Où vit la documentation

- **Confluence** : cahier des charges, DAT et cahier de recettes, versions de référence
- **Jira** (projet PG) : backlog, sprints et tickets ; Sprint 1 = PG-11 et PG-12 (connexion Google)
- **Lucid** : story map, MCD / MLD / MPD, diagrammes UML (cas d'utilisation, séquence, activité, composants, déploiement)
- **Miro** : Product Goal Canvas et équipe projet



## Choix principaux

- **Méthode** : Scrum, sprints de 2 semaines ; la documentation évolue avec chaque sprint (Definition of Done).
- **Stack proposée** : Angular, API Go en monolithe modulaire, PostgreSQL, authentification Google OIDC.
- **Sécurité** : droits vérifiés côté serveur à chaque requête, un seul type d'utilisateur avec des habilitations datées par rôle et promotion.
- **RGPD et accessibilité** : données minimisées et durées de conservation définies, référentiel RGAA 4.1.2.



## Périmètre

Projet de conception : aucun code applicatif n'est livré et aucun test n'a été exécuté. Le Sprint 1 (authentification) est détaillé ; les versions V2 à V4 restent au niveau de la story map.