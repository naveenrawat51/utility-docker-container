# Setup utility-container Docker

### Executing program

```
docker build -t node-util .
docker run -it -v C:\Users\narawat\Desktop\Naveen\utility-docker-container\:/app node-util npm init (we are using bind mouting so whatever we are creating into container will be available on host)
```

after adding 'ENTRYPOINT [ "npm" ]' just run
```
docker build -t node-util .
docker run -it -v C:\Users\narawat\Desktop\Naveen\utility-docker-container\:/app node-util init (we can use init/install direct without npm - npm will be considerd as we are using ENTRYPOINT)

OR

docker run -it -v C:\Users\narawat\Desktop\Naveen\utility-docker-container\:/app node-util install express --save
```
