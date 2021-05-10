# Transformation d'un dossier local en dépôt git

- `git init`: va créer un répertoire caché qui va contenir toutes les infos de l'historique de notre projet

ATTENTION : on n'est pas sensé intervenir directement dans ce dossier, il appartient à git, si on fait des modifs dedans c'est à nos risques et périls

- `git add .` : on ajoute au versionning les fichiers de notre projet. Ainsi, git va surveiller les modifications sur ces fichiers et nous alerter afin qu'on ajoute la version modifiée à l'historique  

- `git commit -m "message"` : on crée une archive du projet en l'état pour l'ajouter à l'historique. On fera attention à mettre un message de description du commit le plus parlant possible afin, en un coup d'oeil, de savoir d'où on en était quand on a créé cette archive

- création d'un dépôt vide sur github. Si on laisse les réglages par défaut, à la validation on obtient une liste des commandes à effectuer dans le terminal afin de relier notre dossier local au repo distant sur github
Par défaut, en local, le repo distant est désigné sous le nom origin

- `git remote add origin adresse_ssh_du_repo` : on indique à git sur quelle adresse distante il devra envoyer le code (https ou ssh)

- `git push -u origin nom_branche` : par défaut, la branche principal d'un repo github d'appelle master. Une lubie récente de microsoft propose de la renommer en main pour éviter un terme tendancieux. A vous de voir si vous voulez le faire ou pas  
- Lors du 1er push, on doit préciser l'option -u suivie du nom du dépôt (origin) et du nom de la branche  
- Pour les pushs suivant, on pourra juste utiliser `git push`