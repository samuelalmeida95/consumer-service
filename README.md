# consumer-service

Este projeto é um exemplo simples de como utilizar o RabbitMQ para consumir mensagens em um cenário de microsserviços.

## Requisitos

Para executar o projeto, é necessário ter o Docker e o Docker Compose instalados.

## Como executar

1. Clone este repositório: `git clone https://github.com/samuelalmeida95/consumer-service.git`
2. Acesse o diretório do projeto: `cd consumer-service`
3. Inicie os containers do RabbitMQ e do aplicativo com Docker Compose: `docker-compose up -d`
4. Execute o aplicativo: `./mvnw spring-boot:run`

## Funcionamento

Este projeto consiste em um aplicativo Spring Boot que consome mensagens de uma fila do RabbitMQ.

O aplicativo utiliza a anotação `@RabbitListener` para escutar a fila `product.log` do RabbitMQ. Quando uma mensagem é recebida, o aplicativo exibe um log com a mensagem.

O RabbitMQ é executado em um contêiner Docker separado, com suas configurações definidas no arquivo `docker-compose.yml`.

## Licença

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo `LICENSE` para obter detalhes.

