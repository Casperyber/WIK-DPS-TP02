Tout d'abord il faut commencer par faire un dockerfile, comme celui-ci que j'ai push dans le dépôt.
Ensuite il faut allumer le docker desktop en fond et que vous êtes connecté a votre compte pour que cela fontionne, une fois qu'il est up faites ce qui suit.
Dirigez vous dans le dossier du projet qui est pour moi api.
            - cd C:\chemin\vers\API
Puis nous allons build celui-ci
            - docker build -t api .
Une fois qu'il est build, nous devons le lancer 
            - docker run -d -p 8080:8080 --name monapi api
Une fois qu'il est lancé il faut vérifier qu'il fonctionne et qu'il est bien actif 
            - docker ps
Maintenant testons le 
            - curl http://localhost:8080/ping
Il est maintenant prêt et actif 

Pour pousser la vérification au max en allant directement sur le docker desktop et vérifier que votre projet est build 

