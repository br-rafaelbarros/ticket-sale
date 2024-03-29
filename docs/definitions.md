## Funcionalidades - [(Voltar ao README)](../README.md)
- Mostrar os ingressos disponíveis.
- Gerar um dado de pagamento (PIX), para simular o pagamento dos ingressos.
- Enviar o dado de pagamento para o email do usuário.
- Mostrar os ingressos comprados pelo usuário e seus respectivos status.

## Fluxo principal - [(Voltar ao README)](../README.md)
  A partir da descrição das funcionalidades, foi desenvolvido um diagrama de sequência para representar o fluxo principal do sistema e pode ser encontrado clicando [aqui](./docs/sequence-diagram.md).

## Banco de dados - [(Voltar ao README)](../README.md)
  Por se tratar se um fluxo simples e como demonstração não foi levantado muitas hipóteses de uso para melhor definir o banco de dados, o formato do banco de dados foi o relacional, para facilitar o entendimento da solução aplicada.
  > 📝 ***Obs.: Pelo mesmo motivo de ser um projeto de demonstração, não foi aplicado as melhores práticas de modelagem de banco de dados, como normalização e otimização de queries já que o foco é a demonstração do fluxo principal.***
  
  A solução de banco de dados pode ser encontrada clicando [aqui](./docs/database.md).

## Arquitetura - [(Voltar ao README)](../README.md)
  Sobre a a arquitetura, foi definida uma arquitetura relativamente simples mas bem divida em camadas, pois já conseguiremos com esse desenho separar as responsabilidades e facilitar a manutenção e evolução do sistema.
  > 📝 ***Obs.: Apesar de já saber que se fosse aplicar uma solução em um projeto real, deveria ser aplicado algumas medidas de segurança tando na base quanto na arquitetura como idempotência, rate limit, autenticação e autorização entre outros pontos que devem ser avaliado para o cenário, mas como o projeto é para fins de portifólio e didatico não nos preocuparemos com isso.***

  O desenho da arquitetura pode ser encontrado clicando [aqui](./docs/architecture.md).

## Tecnologias - [(Voltar ao README)](../README.md)
  As tecnologias utilizadas para o desenvolvimento do projeto forma escolhidas para demonstrar conhecimentos em tecnologias atuais e que estão em alta no mercado.
de modo que podemos destacar algumas delas:
  - **Linguagem de programação:** Java 17
  - **Framework:** Spring Boot
  - **Banco de dados:** PostgreSQL
  - **Orquestrador de fila:** Apache Kafka
  - **Gateway de pagamento:** Nenhum, será mockado na camada de serviço externo.
  - **Email provider:** Nenhum, será mockado na camada de serviço externo.
  
  Além dessas tecnologias, estaremos utilizando outras ferramentas para facilitar o desenvolvimento e testes, como por exemplo, Docker, Docker Compose, Testcontainers, Junit, Mockito, entre outros, Lombok etc.
