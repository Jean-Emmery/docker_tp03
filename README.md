# docker_tp03

# 2. Pod Nginx <br>
**a. Héberger un premier Pod Nginx**<br>
  ```kubectl create -f nginx-pod.yaml```<br>

**b. A l’aide de la commande kubectl port-forward et d’un navigateur accéder à la page par défaut de votre pod Nginx**<br>
  ```kubectl port-forward pods/nginx-pod 8080:80```<br>
  ```http://localhost:8080/```<br>

# 2. Connexion entre plusieurs Pods <br>






