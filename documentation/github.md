######      Définition de Git et Github
          
 `git: logiciel qui gère la gestion des versions de code source
 
 `github`: service cloud pour l'hébergement à distance de repo git
  
 
  création un nouveau dossier
 `git init`

        cloner un dépôt
        
 créez une copie de votre dépôt local en exécutant la commande
 
 `git clone /path/to/repository`   
 
 
si vous utilisez un serveur distant, cette commande sera`

 git clone username@host:/path/to/repository`

           
           ajouter & valider`
           
vous pouvez proposer un changement (l'ajouter à l'Index) en exécutant les commandes

`git add <filename>`

`git add *`                                                                                                                                                                                                                                                     

Pour valider ces changements, utilisez

`git commit -m "Message de validation"`                                       


        envoyer des changements
    
 Pour les envoyer à votre dépôt distant, exécutez la commande
 
`git push origin master`                                      

Remplacez master par la branche dans laquelle vous souhaitez envoyer vos changements. 



Si vous n'avez pas cloné votre dépôt existant et voulez le connecter à votre dépôt sur un serveur distant, vous devez l'ajouter avec

`git remote add origin <server>`


                  branches
                  
Les branches sont utilisées pour développer des fonctionnalités isolées des autres. La branche master est la branche par défaut quand vous créez un dépôt. Utilisez les autres branches pour le développement et fusionnez ensuite à la branche principale quand vous avez fini.

créer une nouvelle branche nommée "feature_x"

`git checkout -b feature_x`


retourner sur la branche principale

`git checkout master`

supprimer la branche

`git branch -d feature_x`

une branche n'est pas disponible pour les autres tant que vous ne l'aurez pas envoyée vers votre dépôt distant

`git push origin <branch>`
 
         mettre à jour & fusionner

pour mettre à jour votre dépôt local vers les dernières validations, exécutez la commande

`git pull`

pour fusionner une autre branche avec la branche active (par exemple master), utilisez

`git merge <branch>`