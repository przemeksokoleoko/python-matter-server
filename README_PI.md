Steps to build image and push it to docker hub repo:

docker buildx create --use

docker buildx inspect --bootstrap

docker login

docker buildx build --platform linux/arm/v7 -t ${your_docker_hub_user_name}/python-matter-server:latest -f Dockerfile.pi --push .
