- generate proto file
  - `protoc --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative logs.proto`

- docker build -f front-end.dockerfile  -t hovhannesmn/front-end:1.0.1 .
- docker push hovhannesmn/front-end:1.0.1
- docker service ls
- docker service ls
- docker build -f caddy.dockerfile  -t hovhannesmn/micro-caddy:1.0.0 .


- docker swarm init
- docker stack rm myapp
- docker stack deploy -c swarm.yml myapp
- docker swarm leave --force
