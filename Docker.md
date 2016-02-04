
# How to run this demo on Docker

## Install Docker
- [Install Docker](https://www.docker.com/)
- Open a Command Prompt and check if you successfully execute `docker run hello-world`

## Execute sample portal
- `git clone https://github.com/vishalrohilla-okta/portal-war.git`
- `mkdir acme-demo && cd acme-demo`
- `unzip ./portal.war  -d ./sample`
- Edit `./sample/WEB-INF/classes/Oktaconf.properties` for your demo org
- `docker run -it --rm -p 8080:8080 -v $(pwd)/sample:/usr/local/tomcat/webapps/sample tomcat:8.0`
