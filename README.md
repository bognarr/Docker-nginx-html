sudo -s
sudo apt-get update
sudo apt-get install docker.io -y
docker run -p 80:80 -d nginx
touch Dockerfile 
        → Lépj bele(mc) és másold be ezt!:
FROM nginx:alpine
COPY . /usr/share/nginx/html

touch index.html 
        → lépj bele és másold be ezt!:
<!DOCTYPE html>
<html>
<head>
<title>Ez egy oldal</title>
</head>
<body>
      
<h1>Hello World!</h1>
<p>ppp</p>
      
</body>
</html>
cd
docker ps
docker stop „ide azt írd, ami a 80→80/tcp után áll!”
docker container prune    → yes!
docker images webserver-image:v1
docker build -t ng .
docker run -d -p 80:80 --name sajatnev ng
