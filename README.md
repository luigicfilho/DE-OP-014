# DE-OP-014

1) Install docker engine:
```
https://docs.docker.com/engine/install/ubuntu/
```

2) Clone the repository using git:
```
git clone https://github.com/luigicfilho/DE-OP-014.git
```
3) Go to the application branch:
```
git checkout urlshortner-cs
```

4) Go to the solution folder:
```
cd Ada.UrlShortner
```

5) Build the application using docker:
```
sudo docker build -t ada/url-shortner -f Ada.UrlShortner/Dockerfile .
```

6) Check if container image was created:
```
sudo docker image ls
```

7) Run the application and publish it to the 8080 port:
```
sudo docker run -d -p 8080:8080 ada/url-shortner
```

8) Open the browser and check the application running:
```
http://localhost:8080/
```