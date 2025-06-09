# NSS Smart Home

## Clone repository
    git clone git@github.com:MinMin2424/NSS-SmartHome.git

## Update submodules
    git submodule update --init --recursive

## Update a specific submodule
    git submodule update --remote <service_name>

## Starting project
    docker compose down

## Postup spuštění
Ke spuštění není potřeba vytvářet žádnou databázi, protože ji aplikace nepoužívá :)

    docker compose up --build // pro spuštění microservisy  
    mvn clean package -DskipTests // v adresáči client, následně  
    java -jar target/Client-1.jar // pro spuštění klienta, který všechno volá  
