## Getting Started

Framework utilizado: **Quarkus**

Para rodar o projeto:
```bash
$ cd iac
$ docker-compose up -d
```

- **A Products API irá rodar na porta 8081**
- **A Orders API irá rodar na porta 8082**

- Collection do Postman com todos os endpoints:
  [Link para a coleção Postman](https://github.com/rogerrafael7/k2-rci.git/tree/master/docs/k2-RCI.postman_collection.json)

### Project Details

O projeto está dividido em 3 módulos:
- **products-api**: é um sub-módulo do git([k2-rci-api-products](https://github.com/rogerrafael7/k2-rci-api-products)) que contém a API de produtos 
- **orders-api**: é um sub-módulo do git([k2-rci-api-orders](https://github.com/rogerrafael7/k2-rci-api-orders)) que contém a API de pedidos
- **iac**: é um diretório do projeto principal e que contém os arquivos de infraestrutura como o docker-compose.yml


#### Endpoints:
- **Products API**
  - **GET /products** - Lista todos os produtos
  - **GET /products/{id}** - Busca um produto por ID
  - **GET /products/by-ids** - Busca produtos por IDs
  - **POST /products** - Cria um novo produto
  - **PATCH /products/{id}** - Atualiza um produto
  - **DELETE /products/{id}** - Deleta um produto

- **Orders API**
  - **GET /orders** - Lista todos os pedidos
  - **GET /orders/{id}** - Busca um pedido por ID
  - **POST /orders** - Cria um novo pedido
  - **PATCH /orders/{id}/status** - Atualiza o status de um pedido
  - **PATCH /orders/{id}/items** - Atualiza os items de um pedido
  - **DELETE /orders/{id}** - Deleta um pedido

