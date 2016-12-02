# Utilisation de Git dans Visual Studio 2015
Ce guide utilisateur porte sur l'utilisation de git dans Visual Studio 2015 au département d'informatique du Cégep. Bien qu'il soit possible d'utiliser le mode commande, le guide portera sur l'interface graphique.

# Cloner un projet existant
Pour obtenir une copie du code source de votre projet, vous devez le "cloner". Dans Visual Studio, cliquez sur l'onglet "Team Explorer" en bas à droite. Assurez-vous d'être dans le sous-menu "Connexions" représenté par l'icône suivante : ![manageconnexion](https://github.com/dinfcll/sachem/blob/master/sachem/_Contribute/wiki/manageconnexion.png)

![teamexplorer](https://github.com/dinfcll/sachem/blob/master/sachem/_Contribute/wiki/teamexplorer.png)

Cliquez sur "Cloner", entrez l'url `https://github.com/dinfcll/sachem.git` du projet, sélectionnez l'endroit où vous souhaitez le sauvearder sur votre ordinateur et cliquez sur le bouton "Cloner".

![cloner](https://github.com/dinfcll/sachem/blob/master/sachem/_Contribute/wiki/Capture.PNG)

Visual Studio aura besoin de votre identifiant Git ainsi que votre adresse courriel. Fournissez-lui les informations demandées selon votre compte Git (le même que dans Rocket.Chat).

Ouvrez le projet en double-cliquant sur le nom du projet et en double-cliquant sur le fichier solution.

![ouvrirsolution](https://github.com/dinfcll/sachem/blob/master/sachem/_Contribute/wiki/ouvrirsolution.png)

Cliquez ensuite sur l'onglet "Explorateur de solutions" pour voir l'arborescence du projet.


# Créer une branche
Les branches permettent de travailler sur une fonctionnalité sans nuire au flux principal, qui lui, se doit d'être fonctionnel en tout temps. Autrement dit, lorsqu'on développe une nouvelle fonctionnalité, on se crée une nouvelle branche. Une fois celle-ci terminée, testée et validée, on fusionne cette branche avec la branche principale envoyant ainsi notre nouvelle fonctionnalité dans la branche principale.

Dans Visual Studio, voici les étapes pour créer une nouvelle branche :
  - Dans Team Explorer, choisissez l'option "Branches".
  - Faites apparaître le menu contextuel (clic droit de la souris) sur la branche parent (exemple : master) à partir de laquelle seront effectués vos modifications. Sélectionnez l'option "Nouvelle branche locale de..."

![nouvellebranche](https://github.com/dinfcll/sachem/blob/master/sachem/_Contribute/wiki/nouvellebranche.png)

  - Inscrivez un nom de branche significatif et cliquez sur le bouton "Créer une branche".

![nouvellebranche_majcours](https://github.com/dinfcll/sachem/blob/master/sachem/_Contribute/wiki/nouvellebranche_majcours.png)


# Envoyer vos modifications sur le serveur
Lorsque vous codez, les modifications sont effectuées localement sur votre machine. Pour sauvegarder ces modifications sur le serveur, vous devez faire un "push". Pour se faire, dans Team Explorer, choisissez l'option Modifications.

![teamexploreraccueil](https://github.com/dinfcll/sachem/blob/master/sachem/_Contribute/wiki/teamexploreraccueil.png)

Inscrivez ensuite une description de la modification apportée, vérifiez les fichiers à inclure (il est possible d'exclure un fichier en choisissant l'option "Exclure" du menu contextuel) et choisissez l'option "Valider et faire un Push" ou "Valider et synchroniser". La deuxième option, en plus de faire d'envoyer votre code sur le serveur, obtient les dernières modifications ayant eu lieu sur la branche en cours.

![modification](https://github.com/dinfcll/sachem/blob/master/sachem/_Contribute/wiki/modification.png)

Remarque : l'option "Valider" n'envoie pas votre code sur le serveur. Il effectue un point de sauvegarde localement, sur votre machine.



# Fusionner deux branches
Lorsque vous souhaitez obtenir les mises à jour d'une branche (exemple : la master), dans votre branche en cours, vous devez effectuer une fusion de branche. Attention cependant de l'effectuer dans le bon sens sous peine d'envoyer votre code dans l'autre branche.

Pour importer les modifications d'une branche dans la vôtre, choisissez l'option Branches dans Team Explorer. Sélectionnez ensuite l'option "Fusionner", ce qui donnera le résultat suivant :

![fusionnerbranche2](https://github.com/dinfcll/sachem/blob/master/sachem/_Contribute/wiki/fusionbranche_etape2.png)

La section "Fusionner à partir de la branche" vous permet de sélectionner la branche qui sera importée dans la seconde, soit la section "Dans la branche actuelle". Dans l'écran précédent, les mises à jour de la branche master seront répliquées dans la branche "maj_Cours". Il ne reste qu'à cliquer sur le bouton "Fusionner".

Auteur: Josée Lainesse