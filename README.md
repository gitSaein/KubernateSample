
###1. docker
docker pull tomcat

docker run -d --name tomcat_test -p 80:8080 tomcat

kubectl apply -f service.yaml

####2. pod 배포 
docker login -u=${username} -p=${password} docker.io


docker tag {{username}}//{{imagename}}:{{version}}


docker push {{username}}//{{imagename}}:{{version}}

#####2.1 deployment

https://blog.voidmainvoid.net/122

####3. 컨트롤러를 이용해서 파드 관리




####4. 서비스: 해당 파드에 접근




####5. 인그레스: 클러스터 외부에서 안으로 접근하는 요청 처리

git clone https://github.com/kubernetes/ingress-nginx.git



####6. blue & green deploy

https://www.youtube.com/watch?v=jxhpTGQ484Y