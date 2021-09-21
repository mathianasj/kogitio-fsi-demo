# Local Development
1. first show the spring boot example
    1. cd spring-kogito
    1. mvn spring-boot:run
    1. show startup time
    1. show the swagger-ui http://localhost:8080/swagger-ui/index.html?configUrl=/v3/api-docs/swagger-config
1. show the difference in startup times
    1. cd ../quarkus-kogito
    1. java -jar ./bin/quarkus-kogito-1.0.0-SNAPSHOT-runner.jar
    1. show startup time
    1. show the swagger-ui http://localhost:8080/q/swagger-ui/
    1. demonstrate native ./bin/quarkus-kogito-1.0.0-SNAPSHOT-runner
    1. show the swagger-ui http://localhost:8080/q/swagger-ui/
1. show the quarkus example dev example
    1. cd ../quarkus-kogito
    1. mvn quarkus:dev
    1. demonstrate creation of a new dmn
    1. show that it live updates
1. show testing
    1. show the test scenario
    1. run the vs code test

# Kubernetes
1. Commit the change and show that the github actions is running a pipeline
1. Show existing does not list new dmn in swagger ui
    1. http://dm-demo.example.com/q/swagger-ui
1. Restart the deployment
    1. kubectl rollout restart deployment/decision-deployment  