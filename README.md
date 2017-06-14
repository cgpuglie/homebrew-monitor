# Homebrew Monitor

An Microservice based IOT monitor for homebrewing. Gather statistics from sensors attached to a raspberry pi.

Will deploy to Docker Swarm on Google's GCE using my [GCE Docker Swarm automation](https://github.com/cgpuglie/GCP-Terraform-DockerSwarm) and possibly to Kubernetes on Google's GKE. This repository will house the kubernetes yaml files, Docker stack-files, Integration tests, and CircleCI configs to Test and release this code in an automated fashion.
### Microservice Repositories
This app is made up of a variety of microservices running in Docker containers. Each microservice is versioned independently, and contains unit tests that simulate the interaction between services.

Here are the repositories:

#### Work In Progress
[homebrew-monitor-auth](https://github.com/cgpuglie/homebrew-monitor-auth): Provides APIs to authenticate and authorize an admin user.   
[homebrew-monitor-rest](https://github.com/cgpuglie/homebrew-monitor-rest): Provides REST apis to accept and report statistics from Raspberry Pi's sensors.

#### Future releases
**Raspberry Pi Agent**: Application to gather data from Raspberry Pi's sensors and send to REST API.  
**Google Assistant Actions**:  Google Assistant app to answer questions about homebrews status.  
**Socket API**: Provide realtime subscription data to be consumed by UIs.  
**VueJS UI**: Provide realtime graphs of homebrew stats.

#### Usage documentation to come!