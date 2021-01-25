
# Pre-Requisites
    Four EC2-Instances ( 2 Masters and 2 slaves)    
    Install Docker
# Master1:
  Initilize Docker Swarm Master using below command
  
    docker swarm init
  ![image](https://user-images.githubusercontent.com/58024415/105666025-52df4480-5efe-11eb-83a4-7c678d9471d0.png)
# Provide Alltraffic in security group of master server1
# Provide token number in two slave servers
    docker swarm join --token SWMTKN-1-665j67q59m9nvejhhjx3nfkl8efc0mrv05r032zbfeq4bg2v8f-4kdcrdm3r83dfpgvhpu8ubza7 172.31.56.19:2377
  Node1:
  
  ![image](https://user-images.githubusercontent.com/58024415/105666093-815d1f80-5efe-11eb-82fc-15fa0e2e3b68.png)
  
  Node2:
  
  ![image](https://user-images.githubusercontent.com/58024415/105666110-8d48e180-5efe-11eb-8a84-88d86989e982.png)
# Check token for Master server1 using below command
    docker swarm join-token manager
  ![image](https://user-images.githubusercontent.com/58024415/105666180-b5384500-5efe-11eb-99a4-5e8cbc2d8900.png)
# Provide tocken number in 2nd Master server
    docker swarm join --token SWMTKN-1-665j67q59m9nvejhhjx3nfkl8efc0mrv05r032zbfeq4bg2v8f-b848s67x9xgf8vxfoghekoj32 172.31.56.19:2377
  ![image](https://user-images.githubusercontent.com/58024415/105666237-d39e4080-5efe-11eb-9d3d-fb18860d3c8e.png)
# Check nodes in both master servers
    docker node ls
  Master1:
  
  ![image](https://user-images.githubusercontent.com/58024415/105666294-f29cd280-5efe-11eb-93fb-5f022f3af356.png)
  
  Master2:
  
  ![image](https://user-images.githubusercontent.com/58024415/105666304-fb8da400-5efe-11eb-93ec-a24744607d21.png)
