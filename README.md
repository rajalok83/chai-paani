- #Use below command from project root directory to build docker image

`docker build --rm -t chai-app --file .docker/Dockerfile .`
- #Use below command to check docker images

`docker images -a`
- #Use below command run docker image

`docker run --rm --network host --name my-chai-php chai-app`
- #Use below command to check docker containers running

`docker ps -a`
- #Use below command to delete an images(add option -f at end to forcibly remove image)

`docker images -a | grep -e "none" -e "chai-app" | awk '{print $3}' | xargs docker rmi`
- #Use below command to stop the container

`docker ps | grep "my-chai-php" | awk '{print $1}' | xargs docker stop`
