# GDP

Transformer un email de demande client (quelques lignes seulement) en cahier des charges

## les étapes

- étape 0 : demande d'un client, un appel d'offre, ...
- étape 1 : traduire la demande en use cases (cas d'utilisation) : phrases formalisées qui décrivent les fonctionnalités attendues
- étape 2 : prioriser et organiser les use cases en sprint : étape de développement (dev d'une fonctionnalité) sur une période définie (en général, un sprint s'étale sur une semaine/15 jours)
- étape 3 : maquettage de l'interface (wireframes)

## etape 0 : la demande du client

> Bonjour, nous sommes une école qu'elle est bien, et nous voulons un outil pour faciliter les contacts entre étudiants.  
Nous aimerions donc pouvoir **lister les promotions** ainsi que **les étudiants qui les composent**, 
mais aussi accèder aux **détails d'un étudiant**, photo de profil comprise.  
L'accès aux profils serait libre et gratuit.  
Dans un second temps l'outil pourrait servir à **éditer les profils et promotions**.  
En ésperant que vous pourrez répondre favorablement à notre demande,  
Cordialement  
Nicole.

## etape 1 : Use cases

On traduit la demande en fonctionnalités atomiques (granulaires) implémentables

|#|En tant que ...|Je veux ...|Afin de ...|sprint
|---|---|---|---|---
|1|visiteur|accéder à la page d'accueil|voir les fonctionnalités disponibles sur le site (quasi universel)|1
|2|visiteur|accéder à la liste des promos|voir les promos|1
|3|visiteur|accéder aux détails d'une promo|voir les étudiants qui la composent|1
|4|visiteur|accéder aux détails d'un étudiant|voir son profil|1
|5|visiteur|accéder à un formulaire d'inscription|devenir étudiant ou administrateur|2
|6|visiteur|accéder à un formulaire de login|me connecter|2
|7|etudiant|accéder à mon profil|pouvoir le modifier/supprimer|2
|8|administrateur|accéder à une page sécurisée|effectuer les actions d'administrateur|3
|9|administrateur|accéder à une page d'édition des promos|ajouter/modifier/supprimer une promo|3
|10|administrateur|accéder à une page d'édition des étudiants|ajouter/supprimer un étudiant|3
|11|administrateur|accéder à une page de gestion des utilisateurs|ajouter/modifier les droits des utilisateurs inscrits|3

visiteur : un utilisateur non enregistré ou non loggué  
étudiant : un utilisateur connecté  
administrateur : un utilisateur connecté avec des droits supplémentaires  
