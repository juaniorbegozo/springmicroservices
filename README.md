# POC for Spring boot + spring cloud (service discovery + load balancing + circuit breaker) running on docker swarm mode

- docker build -f Dockerfile.build.local -t eureka-zuul .
- docker build -f Dockerfile.build.local -t eureka-server .
- docker build -f Dockerfile.build.local -t eureka-auth .
- docker build -f Dockerfile.build.local -t eureka-gallery .
- docker build -f Dockerfile.build.local -t eureka-image .
- docker stack deploy springmicroservices --compose-file docker-compose.yml
