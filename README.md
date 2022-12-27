# Docker Demo

Source code from an introductory presentation on Docker that I made. As a hands-on, we containerised a basic Spring application with Java 17 and Maven.


## Instructions
Clone this repository and enter it.
```bash
  git clone https://github.com/stautisabela/docker-demo.git
  cd docker-demo/docker-demo
```
Build the application. If you don't have maven you can mannually do it on your IDE.
```bash
  mvn install
```

Create a Docker image from our project.
```bash
  docker build -t spring-docker-demo.jar .
```

Create a container based on our new image.
```bash
  docker run -p 9090:8080 spring-docker-demo.jar
```

Now you can access your application on [localhost:9090](http://localhost:9090) :smiley:
