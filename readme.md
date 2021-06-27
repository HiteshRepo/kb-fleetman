## Queue

Image : richardchesterwood/k8s-fleetman-queue:release2
Port 8161 : Expose to browser via 30010
Port 61616 : send/recieve message

## Position Simulator

Image : richardchesterwood/k8s-fleetman-position-simulator:release2
Environment Variable : SPRING_PROFILES_ACTIVE : production-microservices

## Position Tracker

Image : richardchesterwood/k8s-fleetman-position-tracker:release2
Port 808 : Test the rest interface
Environment Variable : SPRING_PROFILES_ACTIVE : production-microservices

## API Gateway

Image : richardchesterwood/k8s-fleetman-api-gateway:release2
Port 8080 : Expose to cluster
Environment Variable : SPRING_PROFILES_ACTIVE : production-microservices

## Frontend

Image : richardchesterwood/k8s-fleetman-webapp-angular:release2
Port 80 : Expose this to outside world.
Environment Variable : SPRING_PROFILES_ACTIVE : production-microservices
