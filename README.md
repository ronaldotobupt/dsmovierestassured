# DsMovie - testes utilizando biblioteca RestAssured
●	REST Assured é uma biblioteca usada para automatizar testes de API em aplicações, permitindo testar e validar serviços REST de uma forma simples

# Testes realizados

## Consultar produto por id
Foi implementado um teste de API usando o REST Assured para consultar produto com id existente. Para o teste, foi realizada  uma requisição do tipo GET, no endpoint /products/{id}

## Consultar produtos
Considerando os seguintes cenários:
  1.	Busca paginada exibe listagem paginada de produtos
  2.	Busca paginada filtra produtos por nome e exibe listagem paginada quando campo nome preenchidos

## Inserir produto
Considerando os seguintes cenários:
  1.	Inserção de produto insere produto com dados válidos quando logado como admin
  2.	Inserção de produto retorna 422 e mensagens customizadas com dados inválidos quando logado como admin e campo name for inválido
  3.	Inserção de produto retorna 422 e mensagens customizadas com dados inválidos quando logado como admin e campo description for inválido
  4.	Inserção de produto retorna 422 e mensagens customizadas com dados inválidos quando logado como admin e campo price for negativo
  5.	Inserção de produto retorna 422 e mensagens customizadas com dados inválidos quando logado como admin e campo price for zero
  6.	Inserção de produto retorna 422 e mensagens customizadas com dados inválidos quando logado como admin e não tiver categoria associada
  7.	Inserção de produto retorna 403 quando logado como cliente
  8.	Inserção de produto retorna 401 quando não logado como admin ou cliente



 
