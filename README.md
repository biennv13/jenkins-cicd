link hướng dẫn https://medium.com/@jinvishal2011/kaniko-build-docker-build-in-kubernets-3a1553b928ba

Để sử dụng Kaniko thì phải tạo secret **regcred** nhập thông tin repo (như harbor, docker) và user password
kubectl create secret \
    docker-registry regcred \
    --docker-server=https://index.docker.io/v1/ \
    --docker-username=$REGISTRY_USER \
    --docker-password=$REGISTRY_PASS \
    --docker-email=$REGISTRY_EMAIL
