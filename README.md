# Simple API Rest JAVA Web Service with JAX-RS

## Install in Mac :

```
brew install openjdk

brew search java

brew info java

#If you need to have openjdk first in your PATH, run:
#  echo 'export PATH="/opt/homebrew/opt/openjdk/bin:$PATH"' >> ~/.zshrc

brew install maven
```

## Compile

```
mvn clean -f "./pom.xml"

mvn package -f "./pom.xml"
```

## Execute in Docker

```
# Create docker image with Tomcat 9 and WAR
docker image build -t ortiz/simple_webapp ./

# List docker images
docker image ls

# Creating and running a container
docker container run -it --publish 8082:8080 ortiz/simple_webapp
```

## Test in Browser

URL Test Tomcat admin :

http://localhost:8082


http://localhost:8082/simple_webapp/index.jsp

http://localhost:8082/simple_webapp/rest/hello/Paco





