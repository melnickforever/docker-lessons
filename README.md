# docker-lessons

## Lesson 2: cocker-compose 

Compose is a tool for defining and running multi-container Docker applications. 
With Compose, you use a YAML file to configure your application’s services.  
Then, with a single command, you create and start all the services from your configuration. 
## Features
 Multiple isolated environments on a single host.
 
 Preserve volume data when containers are created
 
 Only recreate containers that have changed

 Common use cases
 
 Development environments
 
 Automated testing environments
 
 ## Network
 Network Drivers
 
 bridge: The default network driver. If you don’t specify a driver, this is the type of network you are creating. Bridge networks are usually used when your applications run in standalone containers that need to communicate. 
 
 host: For standalone containers, remove network isolation between the container and the Docker host, and use the host’s networking directly.
 
 overlay: Overlay networks connect multiple Docker daemons together and enable swarm services to communicate with each other. You can also use overlay networks to facilitate communication between a swarm service and a standalone container, or between two standalone containers on different Docker daemons. This strategy removes the need to do OS-level routing between these containers
 
 macvlan: Macvlan networks allow you to assign a MAC address to a container, making it appear as a physical device on your network.
 
 Network plugins: You can install and use third-party network plugins with Docker
 
 More about docker-compose : https://docs.docker.com/compose/compose-file/