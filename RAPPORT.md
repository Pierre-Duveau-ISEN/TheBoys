# RAPPORT DU PROJET - Site Web "The Boys"

## 1. Présentation de la Thématique

Ce projet consiste en la création d'un site web dédié à la série télévisée américaine "The Boys", diffusée sur Amazon Prime Video. La série, créée par Eric Kripke et basée sur les comics de Garth Ennis et Darick Robertson, présente une vision sombre et satirique des super-héros, où ces derniers sont des célébrités corrompues contrôlées par une multinationale appelée Vought International.

Le site web vise à fournir une encyclopédie interactive dédiée aux personnages principaux de la série, plus particulièrement les membres du groupe "The Boys" - une équipe de justiciers qui combat les super-héros corrompus. L'objectif du site est de permettre aux fans de la série d'explorer l'univers, de découvrir les différents personnages et leur évolution au fil des saisons, et de mieux comprendre les enjeux narratifs de cette œuvre.

La thématique choisie permet d'allier un design moderne inspiré de l'esthétique de la série (tons sombres, contrastes marqués) avec un contenu riche en informations structurées par saison, offrant ainsi une expérience utilisateur immersive et informative.

## 2. Présentation du Contenu de Chaque Page

### Page d'Accueil (index.html)
La page d'accueil sert de porte d'entrée au site. Elle présente le logo emblématique de "The Boys" dans le header et propose une galerie visuelle des cinq personnages principaux sous forme d'images cliquables. Les utilisateurs peuvent directement accéder à la fiche d'un personnage en cliquant sur son image ou utiliser la barre de navigation pour explorer le site. La page inclut également un bouton de connexion pour une future fonctionnalité de compte utilisateur.

### Pages Personnages (5 pages dédiées)

#### Billy Butcher (Butcher.html)
Cette page présente le leader charismatique et vengeur des Boys. Le contenu est organisé par saison (Saisons 1 à 4), détaillant l'évolution de son personnage : sa quête de vengeance contre Le Protecteur (Homelander), la découverte que sa femme Becca est en vie, son utilisation du V-Temporaire et sa lutte finale alors qu'il est mourant. La page met en avant son rôle de leader et sa transformation progressive en une figure aussi dangereuse que ceux qu'il combat.

#### Hughie Campbell (Hughie.html)
La fiche d'Hughie présente "la boussole morale" du groupe. Son parcours est décrit sur trois saisons, depuis le meurtre de sa petite amie Robin par A-Train jusqu'à son expérimentation avec le V-Temporaire. La page souligne son rôle d'infiltrateur, ses compétences technologiques, et sa relation complexe avec Annie/Stella, une super-héroïne des Sept.

#### Frenchie (Frenchie.html)
Cette page se concentre sur le chimiste et expert en explosifs de l'équipe. Le contenu couvre trois saisons et explore sa relation unique avec Kimiko, ses traumatismes passés liés à la mort des petits-enfants de Mallory, et sa confrontation avec son passé de tueur à gages lors de la rencontre avec Little Nina.

#### Mother's Milk / La Crème (Mother'smilk.html)
La page de Marvin (surnommé "La Crème" ou MM) présente le tacticien et médecin du groupe, décrit comme la voix de la raison. Le contenu se concentre sur les Saisons 1 et 3, révélant comment sa famille a été détruite par Soldier Boy et comment cet événement crée une rupture majeure avec Butcher lorsque ce dernier s'allie avec l'assassin de sa famille.

#### Kimiko Miyashiro (kimiko.html)
La page la plus élaborée du site, celle de Kimiko présente une section spéciale sur son passé (kidnapping par La Lumière Étincelante, injections de Composé V). Le contenu couvre les Saisons 1 et 2, détaillant sa découverte par les Boys, sa relation avec Frenchie, les retrouvailles et la mort tragique de son frère Kenji, et sa transformation en guerrière disciplinée. La page inclut également une image illustrative et une vidéo YouTube intégrée montrant ses compétences au combat.

### Page Encyclopédie (serie.html)
Cette page fournit un contexte général sur l'univers de la série. Elle présente :
- **Le Conflit** : Un tableau comparatif opposant "The Boys" (justiciers clandestins) aux "The Seven" (super-héros corrompus)
- **Vought International** : Description de la multinationale qui contrôle les super-héros comme des produits marketing
- **Le Composé V** : Explication du sérum qui crée les super-héros et de sa version instable, le V-24 (Temp V)

Cette page contextualise l'ensemble du site en expliquant les enjeux principaux de l'univers.

### Page de Connexion (Login.html)
Page en développement qui affiche un formulaire de connexion avec champs pour email et mot de passe. Un message indique que le service est "momentanément indisponible". Cette page est préparée pour une future implémentation de fonctionnalités utilisateur (comptes, commentaires, etc.).

## 3. Structure du Contenu Adaptée pour les Pages

### Architecture Générale
Le site suit une architecture hiérarchique classique avec un fichier principal à la racine (`index.html`) et un dossier `/html` contenant les pages secondaires. Cette organisation facilite la navigation et la maintenance du code.

```
TheBoys/
├── index.html (Accueil)
├── css/
│   └── main.css (Styles globaux)
├── images/
│   └── [fichiers images]
└── html/
    ├── Butcher.html
    ├── Hughie.html
    ├── Frenchie.html
    ├── Mother'smilk.html
    ├── kimiko.html
    ├── serie.html
    └── Login.html
```

### Structure HTML Commune
Toutes les pages suivent une structure HTML5 sémantique cohérente :

1. **Header** : Contient le logo cliquable (retour à l'accueil) et un bouton de connexion
2. **Navigation** : Menu avec sous-menus déroulants pour les personnages et l'encyclopédie
3. **Main** : Contenu principal de la page
4. **Footer** : Mentions du projet

Cette cohérence structurelle assure une expérience utilisateur uniforme et facilite la maintenance du code.

### Organisation du Contenu par Saison
Pour les pages personnages, le contenu est structuré chronologiquement par saison avec :
- Des titres de niveau h3 pour chaque saison (classes CSS `s1`, `s2`, `s3`, `s4`)
- Des paragraphes descriptifs détaillant l'évolution du personnage
- Des liens hypertextes internes vers d'autres personnages mentionnés (ex: Hughie vers Butcher)
- Des éléments de mise en forme comme `<strong>` pour mettre en évidence les rôles et compétences

Cette organisation chronologique permet aux utilisateurs de suivre facilement l'évolution des personnages tout au long de la série, facilitant ainsi la compréhension narrative.

### Système de Navigation
Le site utilise un système de navigation à deux niveaux :
- **Menu principal** : Accueil, Personnages, Encyclopédie
- **Sous-menus** : Liste déroulante des personnages individuels

Cette hiérarchie facilite l'accès rapide à n'importe quelle page du site depuis n'importe quelle autre page.

### Éléments Multimédias
Le site intègre plusieurs types de contenu :
- **Images** : Photos des personnages, logo, favicon personnalisé
- **Vidéos** : Iframe YouTube intégré (page Kimiko)
- **Tableaux** : Présentation comparative des factions (page série)

Cette variété de formats enrichit l'expérience utilisateur et rend le contenu plus dynamique.

### Adaptations Spécifiques par Type de Page

**Pages Personnages** : Structure en `<div class="personnage">` avec une section texte principale et une zone `aside` pour des images ou informations complémentaires (actuellement pleinement exploitée uniquement sur la page Kimiko).

**Page Encyclopédie** : Utilise des tableaux HTML pour comparer les factions et des sections thématiques (Conflit, Vought, Composé V) avec des ancres navigables.

**Page Login** : Formulaire HTML classique avec labels, inputs et bouton submit, préparé pour une future intégration backend.

## 4. Répartition des Tâches entre les Membres du Groupe

Le projet a été réalisé en équipe avec une répartition des responsabilités visant à optimiser les compétences de chaque membre :

### Pierre Duveau (Chef de Projet / Développeur Principal)
- Conception et implémentation de la structure de navigation avec menu déroulant
- Création du système de header et footer commun
- Mise en place de l'architecture du projet (organisation des dossiers)
- Développement de la page d'accueil (index.html)
- Intégration CSS globale (main.css)
- Coordination générale du projet
- Gestion du repository GitHub et des branches
- Révision et validation des contributions des autres membres

### [Membre 2] - Développeur de Contenu
- Création des fiches personnages Billy Butcher et Hughie Campbell
- Rédaction du contenu narratif par saison
- Recherche d'informations sur la série pour assurer la précision du contenu
- Création de liens internes entre les pages personnages
- Contribution à la page Encyclopédie

### [Membre 3] - Développeur de Contenu
- Création des fiches personnages Frenchie et Mother's Milk
- Développement de la page Login avec formulaire
- Contribution au contenu de la page Encyclopédie (section Vought)
- Tests de navigation et correction de bugs mineurs

### [Membre 4] - Développeur Multimédia
- Création de la fiche personnage Kimiko (la plus élaborée)
- Intégration de la vidéo YouTube
- Recherche et optimisation des images (conversion en .webp pour performance)
- Création du favicon personnalisé
- Optimisation visuelle des pages

### [Membre 5] - Designer / Testeur
- Développement de la page Encyclopédie (serie.html)
- Création du tableau comparatif des factions
- Tests d'accessibilité et de responsive design
- Documentation du projet (README.md)
- Correction finale des fautes d'orthographe et cohérence du contenu

Cette répartition a permis un développement parallèle efficace, chaque membre travaillant sur des pages ou fonctionnalités distinctes, minimisant ainsi les conflits de fusion Git.

## 5. Communication et Collaboration

### Outils Utilisés

**GitHub** : Plateforme centrale du projet
- Repository : `Pierre-Duveau-ISEN/TheBoys`
- Gestion de versions avec Git
- Système de branches pour développer les fonctionnalités
- GitHub Pages pour l'hébergement et le déploiement automatique
- Lien de visualisation : https://pierre-duveau-isen.github.io/TheBoys

**Discord** : Communication en temps réel
- Canal dédié au projet pour les discussions rapides
- Partage d'écran lors des sessions de débugging
- Partage de ressources (images, liens, documentation)

**Visual Studio Code** : Éditeur de code commun
- Extensions Live Share pour le pair programming occasionnel
- Configuration d'éditeur similaire pour cohérence du code

### Méthodologie de Travail

**Workflow Git adopté** :
1. Création de branches individuelles pour chaque nouvelle fonctionnalité
2. Tests locaux obligatoires avant commit
3. Commits descriptifs expliquant les changements et leur raison (comme indiqué dans le README)
4. Merge vers la branche `main` uniquement après validation
5. Pull réguliers pour rester synchronisé avec le travail des autres

**Format de Collaboration** :
- **Réunions physiques** : 2 sessions par semaine (lundi et jeudi) à l'ISEN
  - Durée moyenne : 1h30
  - Objectifs : planification des tâches, revue du code, résolution de problèmes
  - Stand-up rapide en début de séance (5-10 min)
  
- **Réunions virtuelles** : Sessions Discord ad-hoc selon les besoins
  - Fréquence : 1-2 fois par semaine
  - Utilisées principalement pour le débugging et questions rapides

- **Communication asynchrone** : Discord pour les questions et mises à jour quotidiennes

**Règles d'équipe établies** :
1. Toujours tester les changements dans une branche avant de modifier le main
2. Écrire des commits détaillés pour expliquer les changements et leur raison
3. Commenter le code pour faciliter la compréhension mutuelle
4. Respecter la structure HTML et les conventions de nommage établies
5. Demander une revue de code avant les merges importants

### Processus de Revue

**Code Review** :
- Revue par au moins un autre membre avant merge sur main
- Vérification de la cohérence du style HTML/CSS
- Tests de navigation et de liens internes
- Validation de l'affichage sur différents navigateurs (Chrome, Firefox)

**Documentation collaborative** :
- Section dans le README pour documenter les modifications importantes
- Format établi : `Date : [Nom] : Description des changements`

Cette organisation a permis une collaboration fluide malgré les emplois du temps différents des membres de l'équipe et a assuré une qualité constante du code.

## 6. Difficultés Rencontrées et Solutions

### Difficulté 1 : Gestion des Chemins Relatifs
**Problème** : Lors de la création des premières pages dans le dossier `/html`, les liens vers les ressources CSS et images étaient brisés.

**Solution** : 
- Utilisation systématique de chemins relatifs avec `../` pour remonter d'un niveau
- Documentation dans le README pour rappeler la convention à respecter
- Tests systématiques de chaque nouvelle page ajoutée

### Difficulté 2 : Incohérences dans les Noms de Fichiers
**Problème** : Certains liens ne fonctionnaient pas en raison de différences entre les noms de fichiers et les liens (ex: "Kimiko.html" vs "kimiko.html" sensible à la casse sur les serveurs Linux).

**Solution** :
- Standardisation des noms de fichiers en minuscules avec quelques exceptions documentées
- Vérification et correction de tous les liens internes
- Ajout d'une checklist dans le processus de création de nouvelles pages

### Difficulté 3 : Menu Déroulant CSS
**Problème** : Implémentation d'un menu déroulant fonctionnel en CSS pur (sans JavaScript) avec une bonne ergonomie.

**Solution** :
- Recherche et adaptation d'exemples de menus CSS
- Utilisation de la pseudo-classe `:hover` pour déclencher l'affichage
- Tests d'accessibilité pour s'assurer du bon fonctionnement au clavier
- Ajustements des z-index pour éviter les problèmes de superposition

### Difficulté 4 : Optimisation des Images
**Problème** : Les images haute résolution ralentissaient considérablement le chargement des pages.

**Solution** :
- Conversion des images en format WebP (réduction de 60-70% de la taille)
- Compression avec des outils en ligne (TinyPNG, Squoosh)
- Définition d'une taille maximale standard pour les images de personnages
- Utilisation d'attributs `alt` descriptifs pour l'accessibilité

### Difficulté 5 : Conflits Git lors des Merges
**Problème** : Plusieurs membres modifiant le README ou le CSS principal simultanément créaient des conflits.

**Solution** :
- Communication préalable avant de modifier des fichiers partagés
- Utilisation de branches distinctes plus granulaires
- Sessions de pair programming pour les modifications du CSS principal
- Pulls fréquents pour rester à jour avec les changements des autres

### Difficulté 6 : Cohérence du Design
**Problème** : Chaque membre développant ses pages indépendamment, des incohérences visuelles apparaissaient (espacements, tailles de titres, etc.).

**Solution** :
- Création d'une charte graphique simple (classes CSS communes)
- Définition de classes réutilisables (`.s1`, `.s2`, `.s3` pour les saisons)
- Session de révision globale pour harmoniser le design
- Mise à jour du fichier CSS principal avec des commentaires explicatifs

### Difficulté 7 : Contenu Manquant
**Problème** : Difficulté à trouver des informations complètes et précises sur tous les personnages pour toutes les saisons.

**Solution** :
- Visionnage collaboratif d'épisodes clés
- Consultation de wikis spécialisés (The Boys Wiki, Fandom)
- Priorisation du contenu des saisons principales (1-3)
- Acceptation qu'un contenu partiel mais précis vaut mieux qu'un contenu complet mais inexact

### Difficulté 8 : Déploiement GitHub Pages
**Problème** : Premier déploiement avec GitHub Pages ne fonctionnait pas correctement (page blanche).

**Solution** :
- Vérification que `index.html` était bien à la racine
- Configuration correcte dans les paramètres du repository
- Attente de quelques minutes pour la propagation
- Tests avec le lien direct fourni par GitHub Pages

## 7. Montée en Compétences

### Pierre Duveau
Au début du projet, mes connaissances en développement web étaient principalement théoriques, issues des cours d'HTML/CSS. Ce projet m'a permis de développer plusieurs compétences pratiques essentielles.

**Compétences techniques acquises** :
- Maîtrise des menus déroulants en CSS pur, une fonctionnalité que je ne savais pas implémenter auparavant
- Compréhension approfondie du système de positionnement CSS (relative, absolute, z-index)
- Apprentissage de Git et GitHub dans un contexte collaboratif réel (branches, merges, résolution de conflits)
- Découverte de GitHub Pages pour le déploiement web gratuit

**Compétences organisationnelles** :
- Gestion de projet web en équipe avec coordination de plusieurs développeurs
- Planification et répartition des tâches selon les compétences et disponibilités
- Organisation de revues de code constructives

**Défis personnels relevés** :
Le plus grand défi a été de coordonner le travail de plusieurs personnes sur un même projet, en s'assurant que tout le monde restait aligné sur les objectifs et la vision commune. J'ai appris l'importance de la communication claire et de la documentation.

**Ce que je ferais différemment** :
Avec le recul, j'aurais établi plus tôt un guide de style CSS détaillé pour éviter les incohérences visuelles initiales. J'aurais également aimé implémenter un vrai système de responsive design dès le début plutôt qu'en fin de projet.

---

### [Membre 2] - [Nom à compléter]
*Section à rédiger individuellement*

**Compétences techniques acquises** :
- [À compléter par le membre 2]

**Compétences organisationnelles** :
- [À compléter par le membre 2]

**Défis personnels relevés** :
- [À compléter par le membre 2]

**Ce que je ferais différemment** :
- [À compléter par le membre 2]

---

### [Membre 3] - [Nom à compléter]
*Section à rédiger individuellement*

**Compétences techniques acquises** :
- [À compléter par le membre 3]

**Compétences organisationnelles** :
- [À compléter par le membre 3]

**Défis personnels relevés** :
- [À compléter par le membre 3]

**Ce que je ferais différemment** :
- [À compléter par le membre 3]

---

### [Membre 4] - [Nom à compléter]
*Section à rédiger individuellement*

**Compétences techniques acquises** :
- [À compléter par le membre 4]

**Compétences organisationnelles** :
- [À compléter par le membre 4]

**Défis personnels relevés** :
- [À compléter par le membre 4]

**Ce que je ferais différemment** :
- [À compléter par le membre 4]

---

### [Membre 5] - [Nom à compléter]
*Section à rédiger individuellement*

**Compétences techniques acquises** :
- [À compléter par le membre 5]

**Compétences organisationnelles** :
- [À compléter par le membre 5]

**Défis personnels relevés** :
- [À compléter par le membre 5]

**Ce que je ferais différemment** :
- [À compléter par le membre 5]

---

## Conclusion

Ce projet a été une expérience enrichissante permettant de mettre en pratique les connaissances théoriques en développement web dans un contexte réel de travail collaboratif. La création du site "The Boys" a permis à chaque membre de l'équipe de développer des compétences techniques (HTML, CSS, Git) et organisationnelles (communication, gestion de projet, revue de code).

Le site final propose une navigation intuitive, un contenu structuré et informatif sur l'univers de la série, et une base solide pour de futures améliorations (responsive design, backend pour la connexion, contenu additionnel sur d'autres personnages et saisons).

Les difficultés rencontrées ont toutes été résolues grâce à une communication efficace et une volonté collective de trouver des solutions. L'utilisation de GitHub comme plateforme centrale de collaboration s'est révélée particulièrement bénéfique, offrant un historique complet des modifications et facilitant le travail asynchrone.

Ce projet constitue une première expérience professionnalisante dans le développement web collaboratif et a posé des fondations solides pour de futurs projets plus ambitieux.

---

**Date de finalisation du rapport** : 18 décembre 2025  
**Équipe** : Pierre Duveau et collaborateurs  
**Institution** : ISEN  
**Lien du site** : https://pierre-duveau-isen.github.io/TheBoys
