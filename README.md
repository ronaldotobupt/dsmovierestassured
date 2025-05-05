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

## Deletar produto
Considerando os seguintes cenários:
  1.	Deleção de produto deleta produto existente quando logado como admin
  2.	Deleção de produto retorna 404 para produto inexistente quando logado como admin
  3.	Deleção de produto retorna 400 para produto dependente quando logado como admin
  4.	Deleção de produto retorna 403 quando logado como cliente
  5.	Deleção de produto retorna 401 quando não logado como admin ou cliente

## Consultar pedido por id
Considerando os seguintes cenários:
  1.	Busca de pedido por id retorna pedido existente quando logado como admin
  2.	Busca de pedido por id retorna pedido existente quando logado como cliente e o pedido pertence ao usuário
  3.	Busca de pedido por id retorna 403 quando pedido não pertence ao usuário
  4.	Busca de pedido por id retorna 404 para pedido inexistente quando logado como admin
  5.	Busca de pedido por id retorna 404 para pedido inexistente quando logado como cliente
  6.	Busca de pedido por id retorna 401 quando não logado como admin ou cliente



 
