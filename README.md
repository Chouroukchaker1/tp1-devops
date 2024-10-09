# tp1-devops
Q1/Si vous avez oublié de créer un fichier README.md lors de l'initalisation du projet,comment pouvez-vous l'ajouter après coup et commiter les changements ?                                          REP:(Créer le fichier README.md ,git add README.md,git commit -m "Ajout du fichier README.md",git push origin main)
Q2/Comment définir un dépôt distant si vous n'en avez pas configuré un lors de la création du projet ?  REP:1/git remote add origin https://github.com/Chouroukchaker/nom_du_depot.git                            2/verification que le dépôt a bien été ajouté:git remote add origin https://github.com/Chouroukchaker1/nom_du_depot.git  avec la commande"git remote -v" et apres en push le projet avec la commande "git push -u origin main"
Q3/Comment annuler les modificatons locales d'un fichier avant de les ajouter à l'index ?            REP:git checkout -- nom_du_fichier
Q4/Comment visualiser les fichiers qui sont prêts à être commités dans Git (staging) ?               REP:git status
Q5/Comment suivre (track) un dépôt distant et récupérer toutes les branches de ce dépôt ?            Récupérer toutes les branches:git fetch origin                                             
 Lister toutes les branches:git branch -a                                                     Suivre une branche distante: git checkout -b feature-branch origin/feature-branch         Récupérer toutes les branches et les créer localement:git checkout --trackorigin/nom_de_branche
Q6/Comment supprimer une branche locale après l'avoir fusionnée dans master ?                       1/je verfie que je suis dans la branche master                                                      git checkout master                                                                         2/Fusionner la branche :                                                                            git merge nom_de_branche                                                                     3/ Supprimer la banche locale                                                                   git branch -d nom_de_branche                                                                     
Q7/Comment interrompre un rebase en cours si vous avez commis une erreur ?                       git rebase --abort                                                                              git rebase nom_de_branche                                                                       
Comment lister les commits qui vont être rebasés avant de lancer un rebase ?                     git rebase --interactive --preview <branche_cible>                                              git log --oneline <branche_cible>..<votre_branche>
Q8/Comment afficher la liste des branches actives et en cours de développement dans Gitlow ?        Afficher les branches principales dans Gitflow:git branch --list master develop                  Lister toutes les branches actives:git branch --list                                            Pour afficher les branches de fonctionnalités actives (feature/*) :git branch --listfeature/*                                                                                    Pour afficher les branches de release :git branch --list release/*                              Pour afficher les branches de correctifs (hotfix/*) :git branch --list hotfix/*                  Lister toutes les branches actives distantes:git branch -r                                      Utiliser git flow pour une vue générale:git flow feature                                    git flow release                                                                            
git flow hotfix
 





    









