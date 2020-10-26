<<<<<<< HEAD

###1. docker
docker pull tomcat

docker run -d --name tomcat_test -p 80:8080 tomcat

kubectl apply -f service.yaml

####2. pod 배포 : 가장 기본적인 배포 단위 컨테이너들을 포함하고 있음
docker login -u=${username} -p=${password} docker.io


docker tag {{username}}//{{imagename}}:{{version}}


docker push {{username}}//{{imagename}}:{{version}}

####3 deployment 컨트롤러: 파드들을 관리하는 역할

https://blog.voidmainvoid.net/122


####4. 서비스: 해당 파드에 접근, 여러 개의 pod들을 서비스할 때, 현재 요청이 어느 pod로 갈지 선택하는 오브젝트
부하가 많을때, 이를 분산 하는 로드밸런서 역할

kubectl apply -f example-blue-service.yaml


kubectl expose deployment example-blue-service --type="NodePort" --port 8081 service example-blue-service expose

####5. 인그레스: 클러스터 외부에서 안으로 접근하는 요청 처리

git clone https://github.com/kubernetes/ingress-nginx.git


kubectl expose deploy deployment/example-blue-service --name service/example-blue-service



####6. blue & green deploy

=======

###1. docker
docker pull tomcat

docker run -d --name tomcat_test -p 80:8080 tomcat

kubectl apply -f service.yaml

####2. pod 배포 : 가장 기본적인 배포 단위 컨테이너들을 포함하고 있음
docker login -u=${username} -p=${password} docker.io


docker tag {{username}}//{{imagename}}:{{version}}


docker push {{username}}//{{imagename}}:{{version}}

####3 deployment 컨트롤러: 파드들을 관리하는 역할

https://blog.voidmainvoid.net/122


####4. 서비스: 해당 파드에 접근, 여러 개의 pod들을 서비스할 때, 현재 요청이 어느 pod로 갈지 선택하는 오브젝트
부하가 많을때, 이를 분산 하는 로드밸런서 역할

kubectl apply -f example-blue-service.yaml


kubectl expose deployment example-blue-service --type="NodePort" --port 8081 service example-blue-service expose

####5. 인그레스: 클러스터 외부에서 안으로 접근하는 요청 처리

git clone https://github.com/kubernetes/ingress-nginx.git


kubectl expose deploy deployment/example-blue-service --name service/example-blue-service



####6. blue & green deploy

>>>>>>> cf11248137102dc93e01ed3b915ea84b88e6e2de
https://www.youtube.com/watch?v=jxhpTGQ484Y