# account-consumer-3
Account Consumer 3

docker network create -d bridge account 
docker network ls  

docker build -t gar2000b/account-consumer-3 .  
docker run -it -d -p 9087:9087 --network="account-consumer-3" --name account-consumer-3 gar2000b/account-consumer-3  

All optional:

docker create -it gar2000b/account-consumer-3 bash  
docker ps -a  
docker start ####  
docker ps  
docker attach ####  
docker remove ####  
docker image rm gar2000b/account-consumer-3  
docker exec -it account-consumer-3 sh  
docker login  
docker push gar2000b/account-consumer-3  