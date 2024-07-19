# API RESTful com Spring Boot, JPA, PostgreSQL, HATEOAS e Postman


#### Este projeto implementa uma API RESTful utilizando Spring Boot, JPA (Java Persistence API), banco de dados PostgreSQL, HATEOAS (Hypermedia as the Engine of Application State) e utiliza o Postman para testes.

Tecnologias Utilizadas
-

- Spring Boot: Framework de desenvolvimento rápido de aplicações para Spring 


- JPA: Fornece mapeamento objeto-relacional para persistência de dados


- PostgreSQL: Sistema de gerenciamento de banco de dados relacional open-source 


- HATEOAS: Estilo arquitetural para APIs REST que inclui links de hipermídia para navegação
    Postman: Ferramenta para testar e documentar APIs

Funcionalidades
- 
- Operações CRUD (Criar, Ler, Atualizar, Deletar) em entidades de produtos
  
  
- Respostas habilitadas para HATEOAS com links para recursos relacionados
 

- Integrado com PostgreSQL para armazenamento de dados

Executando a Aplicação
- 
Pré-requisitos:
    Java 11 ou superior
    Ferramenta de build Maven
    Servidor PostgreSQL rodando na sua máquina local ou em uma instância de banco de dados remota

Clone o Repositório:

    git clone https://github.com/KirinRyu/SistemaCadastroItemCRUD



Construa o Projeto:

    cd SistemaCadastroItemCRUD

    mvn clean install  # Usando Maven

    mvn spring-boot:run  # Usando Maven


A aplicação irá iniciar na porta padrão do Spring Boot (geralmente 8080).

Endpoints da API
-
URL Base: http://localhost:8080 (ou a porta configurada)

POST "/product": Cria um novo registro de produto.
    Corpo da Requisição (JSON):
    JSON

    {
      "name": "Nome do Produto",
      "value": 123.45
    }



GET /product: Recupera todos os registros de produtos.


GET /product/{id}: Recupera um único registro de produto pelo seu ID.


PUT /product/{id}: Atualiza um registro de produto existente.

DELETE /product/{id}: Deleta um registro de produto existente.
    Variável de Caminho: {id} - O identificador único do registro do produto.

Usando o Postman
-
Instale o Postman em https://www.getpostman.com/.
Crie uma nova coleção para sua API.
Defina requisições para cada endpoint e forneça cabeçalhos e corpos de requisição necessários.
Envie requisições e explore respostas com links HATEOAS para navegação e interação adicionais com a API.

Notas Adicionais

Este é um exemplo básico de uma API RESTful com HATEOAS.
Você pode expandir este projeto adicionando mais recursos e funcionalidades.
Certifique-se de configurar os detalhes de conexão do seu banco de dados PostgreSQL no arquivo de propriedades da aplicação (application.properties).