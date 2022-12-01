1. Realizar build da aplicação do Bacen
    1. Abrir o projeto no intelliJ
    2. Executar o comando do Maven: `mvn clean package -Dmaven.test.skip`
    3. Copiar arquivo do diretório onde disponibilizou o target `{{bacen}}\target\bankcode-0.0.1-SNAPSHOT.jar` para `\prometheus\bacen-image\target`
2. Realizar build da aplicação do BankCode
    1. Abrir o projeto no intelliJ
    2. Executar o comando do Maven: `mvn clean package -Dmaven.test.skip`
    3. Copiar arquivo do diretório onde disponibilizou o target `{{bankCode}}\target\bankcode-0.0.1-SNAPSHOT.jar` para `\prometheus\bank-image\target`

3. Criar Dockerfile para bacen

4. Criar Dockerfile para BankCode

5. Criar docker-compose com os serviços:
    - Prometheus (depende dos serviços)
    - Grafana (depende dos serviços)
    - Kafka
    - Mysql
    - Serviços (depende do MySQL e Kafka)

6. Criar Datasource com o nome do container `http://prometheus:9090`

7. Importar dashboard no grafana pelo código

- Material:
https://ordina-jworks.github.io/monitoring/2020/11/16/monitoring-spring-prometheus-grafana.html

https://medium.com/javarevisited/springboot-app-monitoring-with-grafana-prometheus-7c723f0dec15

https://github.com/hugobrendow/lets-microservices/blob/main/Cloud%20%26%20Observability/aula02-prometheus_e_grafana.md

https://github.com/hugobrendow/lets-microservices/blob/main/Cloud%20%26%20Observability/aula02.1-pratica.md

https://github.com/hugobrendow/lets-microservices/blob/main/Cloud%20%26%20Observability/aula02.1-pratica_prometheus.md
