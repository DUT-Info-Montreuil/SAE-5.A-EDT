<div align="center">

# Gestionnaire EDT

**Un site web d'édition d'emploi du temps pour IUT.**<br/>
Réalisé dans le cadre d'une SAÉ ([Situation d'apprentissage et d'évaluation)](https://fr.wikipedia.org/wiki/Situation_d%27apprentissage_et_d%27%C3%A9valuation), ce projet a pour but de faciliter la planification et la création des cours.<br/>
Gestionnaire d'EDT est découpé en trois dépôts : le front-end, l'API et la base de données (**le troisième repo sera créer lors de la semaine de refactor**).


</div>

## 🐳 Comment lancer l'application ?

Prérequis :
- Installer [Docker](https://docs.docker.com/engine/install/)

> [!IMPORTANT]
> Le Makefile sera créé pendant la semaine de refactoring.
> Pour l'instant, exécutez le docker-compose sur le backend et faites tourner le frontend avec *ng-serve*.
> Pour obtenir les données de test, utilisez la route */create_university_db*.

Lancer l'application :

    make

En ajoutant *with-data*, l'application génère un jeu de données vous permettant de l'essayer. Cette option ne doit pas être choisie pour le déploiement, elle vous permet uniquement de prendre en main l'application.

    make with-data

**NB: Nous n'avons pas publié d'image de la release sur Docker Hub Ce choix a été fait car le projet s'il est déployé necessitera d'être remanié.**

## 📆 Comment utiliser l'application ?

Différents rôles existent au sein de l'application ; ceux-ci n'ont pas les mêmes privilèges. [*Veuillez vous référer à la documentation utilisateur pour en savoir plus*]()

> [!IMPORTANT]
> Changer le mot de passe administrateur et la clé d'accès JWT conformément à ce qui est indiqué sur [le README de l'API **link vers la section en question**](https://github.com/DUT-Info-Montreuil/SAE-5.A-EDT-API)
> **Cela ne sera plus nécessaire après la semaine de refactoring. Ces informations seront passées en variables d'environnement.**

Par défaut (*si vous lancez l'application sans générer le jeu de données*), il n'existe qu'un utilisateur. Celui-ci possède le rôle d'administrateur.
Rôle | Login | Mot de passe
---: | :---: | :--- 
**Admin** | admin | admin

Si vous décidez de lancer l'application avec le jeu de données pré-généré.
Rôle | Login | Mot de passe
---: | :---: | :--- 
**Admin** | pbonnot | aA123456789_
**Enseignant Responsable** | mlamolle | aA123456789_
**Enseignant** | gdelmas | aA123456789_
**Etudiant** | hcohen | aA123456789_

Pour obtenir plus d'informations sur le fonctionnement du site web, veuillez consulter la [documentation utilisateur]()

## 🔗 Liens

> [!NOTE]
> Veuillez vous référer au README des dépôts individuels pour obtenir plus d'informations techniques.

Repositories :<br/>
- [API](https://github.com/DUT-Info-Montreuil/SAE-5.A-EDT-API)
- [Front](https://github.com/DUT-Info-Montreuil/SAE-5.A-EDT-Front)

## 🚶 Auteurs

- [@Aldriculteur](https://github.com/Aldriculteur) - Aldric CLAUDE
- [@Lony027](https://github.com/Lony027) - Hugo COHEN
- [@adil93s](https://github.com/adil93s) - Adil CHETOUANI
- [@MehediT](https://github.com/MehediT) - Mehedi TOURE
- [@bseydi](https://github.com/bseydi) - Boulaye SEYDI