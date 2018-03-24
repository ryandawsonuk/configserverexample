# Simple Example of using the Spring Cloud Config Server

Just clone the project and run - no need to set up a config repo to see it work as it takes config from configserver's classpath using native profile

## How to Run

Go configclient directory and do 'mvn spring-boot:run'

Go to localhost:8080 in the browser to see ‘Hello from application properties’.

Go to the configserver directory and do 'mvn spring-boot:run'

Refresh the client with 'curl -X POST http://localhost:8080/actuator/refresh'

Now if we go to localhost:8080 again or refresh that page in the browser we see “Hello from configserver”

## Credits

ASCII Art from http://www.ascii-art-generator.org/ and http://www.writeups.org/optimus-prime-transformers-g1-profile/

