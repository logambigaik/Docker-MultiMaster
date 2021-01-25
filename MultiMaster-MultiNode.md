
# Pre-Requisites
    Four EC2-Instance
    Install Docker
# Master1:
  Initilize Docker Swarm Master using below command
  
      docker swarm init
# Provide tocken number in two slave servers
    docker swarm join --token SWMTKN-1-3enwfizdbcbeq4qcfxwbu4nfhqh9z9mpmn78ocmq42bmzhlzcu-6wzytsk3rs9l2wakepaffvp6n 172.31.88.143:2377
  ![image](https://user-images.githubusercontent.com/58024415/105353991-f3d7b200-5c15-11eb-9561-cf5151dbd605.png)
# Check token for Master server using below command
    docker swarm join-token manager
# Provide Alltraffic in security group of master server
# Provide tocken number in 2nd Master server
  
# Check nodes in Master1 and Master2
    docker node ls
  ![image](https://user-images.githubusercontent.com/58024415/105354101-1964bb80-5c16-11eb-9da5-0a30d95b9ce6.png)
