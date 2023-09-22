build the container
docker build -t myapp:frontend -f Dockerfile.dev .


start the docker container

docker run -p 3000:3000 -v /app/node-modules -v /home/david/Documents/codelabs/docker/grinder/frontend:/app --rm myapp:frontend

docker run --name myapp_frontend_c -p 3000:3000 -v /app/node-modules -v $(pwd):/app --rm myapp:frontend

/home/david/Documents/codelabs/docker/grinder/frontend

<!-- start the  -->
`docker run --name myapp_frontend_prod_c --rm -p 8000:80 myapp:prod`