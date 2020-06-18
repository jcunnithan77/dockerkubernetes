# dockerkubernetes
Docker Commands
  Get Image list : -  docker images
  Build from file :- docker build -f Dockerfile-jenkins-master -t jcunnithan/jenkins-master .
  Docker hublogin :- docker login
  docker hub push:- docker push path

Installation Jenkins over docker 
  Pull jenkin image :-docker pull jenkins/jenkins:lts
  Run jenkin:- docker run --detach --publish 8080:8080 --volume jenkins_home:/var/jenkins_home --name jenkins jenkins/jenkins:lts
  Get Password:- docker exec jenkins cat /var/jenkins_home/secrets/initialAdminPassword
  kubectl -n jenkins port-forward jenkins-778bf9c5cf-skkg5 8080:8080
  
