# Devops-work

#Method-1

Step 1)- copy in “windows cmd” with command
 “git clone https://github.com/ranjitm10/Devops-work.git”
 
Step 2)- Open the folder and run the cmd
 “kubectl apply -k ./”
 
 *Note :- It will take more time to create pods maximum 30min depends on Internet
Speeds.

Step 3)- cmd “git gets pods” its will show ‘creating container’

Step 4)- go to dashboard of k8s

#Method-2

# kubectl.exe create deployment mywp --image=wordpress:5.1.1-php7.3-apache
# kubectl.exe create deployment mydb --image=mysql:5.7
# kubectl.exe set env deployment mydb  --env=MYSQL_USER=ranjit --env=MYSQL_PASSWORD=redhat --env=MYSQL_DATABASE=wpdb --env=MYSQL_ROOT_PASSWORD=123456
#kubectl scale -n default deployment mydb --replicas=10
# kubectl.exe expose deployment mywp --port 80 --type=NodePort
# minikube.exe service mywp

*Note:-
-Change to the deployment should always ensure at least 7 replicas are running at all times.
-There should be 10 replicas running
