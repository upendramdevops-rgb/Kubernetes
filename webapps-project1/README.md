# develop a the application using java code and automate application using jenkins ci/cd pipeline. 
# CI - stages are like checkout, CQA, QG(quality gate), build- application using maven, store artifact, build image, scan-image using trivy, push image to rgistry and update image to manifests.
# CD - stages are checkout and deploy aplication using jenkis.
# for deploy application using a jenkins.
   1. create a service-account for jenkins.
   2. create role (role.yam)
   3. create a rolebinding (rolebinding.yaml)
   4. create secret (secret-token.yaml)

# these resource are created in particular namespace (kubectl apply -f service-account.yaml -n webapps, kubectl apply -f role.yaml -n webapps ) .
# cmnds
 1. kubectl get all -n webapps
 2. kuectl get pos -n webapps
 3. kubectl describe pod podname -n webapps
 4. kubect log podname -n webapps
 5. kubectl log podname -c container-name -n webapps
 6. kubectl log podname -c container-name --previous -n webapps
