# docker_tp03

# 2. Pod Nginx <br>
**a. Héberger un premier Pod Nginx**<br>
  ```kubectl create -f nginx-pod.yaml```<br>

**b. A l’aide de la commande kubectl port-forward et d’un navigateur accéder à la page par défaut de votre pod Nginx**<br>
  ```kubectl port-forward pods/nginx-pod 8080:80```<br>
  ```http://localhost:8080/```<br>

# 3. Connexion entre plusieurs Pods<br>
**a. A l’image du TP 1 sur Docker (question 7 et 8), héberger un Pod phpmyadmin et mysql, cette fois-ci en utilisant minikube**<br>
  ```kubectl apply -f phpmyadmin-mysql-pod.yaml```

**b. Créer un service associé au Pod mysql**<br>

  ```kubectl apply -f service-mysql.yaml```


**c. Connecter phpmyadmin avec le Service mysql et vérifier que vous pouvez administrer cette base de données**<br>


**d. Avec la commande kubectl-port forward, vérifier que phpmyadmin arrive à contacter et administrer votre base de données mysql**<br>
  ```kubectl port-forward phpmyadmin-mysql-pod 8080:80```

**e. Ajouter un Ingress pour accéder à phpmyadmin sans utiliser la commande kubectl port-forward**<br>
  ```kubectl apply -f phpmyadmin-ingress.yaml```
  ```http://phpmyadmin.local/```





