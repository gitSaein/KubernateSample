
###docker
docker pull tomcat

docker run -d --name tomcat_test -p 80:8080 tomcat

kubectl apply -f service.yaml

####pod 배포
docker login -u=${username} -p=${password} docker.io


docker tag {{username}}//{{imagename}}:{{version}}


docker push {{username}}//{{imagename}}:{{version}}
