# API de Gerenciamento de Cidades e Eventos

Este projeto contém uma API REST desenvolvida com Java e Spring Boot, utilizada para gerenciar cidades e eventos. O desafio foca no desenvolvimento de funcionalidades com base no princípio do TDD (Test-Driven Development), onde os testes automatizados são escritos antecipadamente para servir como especificação do comportamento esperado. Além disso, o outro objetivo é implementar uma API RESTful eficiente, com foco no tratamento adequado de exceções e no uso correto dos códigos de status HTTP.

## Funcionalidades da API

### Critérios de Avaliação

#### 1. **`DELETE /cities/{id}`**
- **Descrição**: Exclui uma cidade com base no ID fornecido.
- **Critérios de Correção**:
  - **404 Not Found**: Retorna este código quando o ID da cidade não existe.
  - **204 No Content**: Retorna este código quando a cidade é excluída com sucesso.
  - **400 Bad Request**: Retorna este código quando a cidade é dependente de outros recursos e não pode ser excluída.

#### 2. **`POST /cities`**
- **Descrição**: Cria uma nova cidade.
- **Critério de Correção**: O recurso deve ser inserido corretamente, com retorno adequado.

#### 3. **`GET /cities`**
- **Descrição**: Retorna uma lista de cidades, ordenadas alfabeticamente pelo nome.
- **Critério de Correção**: As cidades devem ser retornadas em ordem alfabética crescente.

#### 4. **`PUT /events`**
- **Descrição**: Atualiza um evento existente com base no ID.
- **Critérios de Correção**:
  - **404 Not Found**: Retorna este código quando o evento não existe.
  - Caso o evento exista, o recurso é atualizado com sucesso.

## Competências Avaliadas

- **Desenvolvimento de API REST com Java e Spring Boot utilizando TDD**: O aluno será avaliado pela capacidade de aplicar TDD no desenvolvimento da API, garantindo que os testes sejam escritos antes do código e validem os requisitos de cada funcionalidade.
  
- **Implementação de cenários de busca, inserção, deleção e atualização de recursos**: O aluno deverá implementar funcionalidades robustas para realizar a manipulação de dados, incluindo as operações CRUD (Create, Read, Update, Delete).
  
- **Tratamento de exceções e respostas HTTP customizadas**: A API deve ser capaz de retornar códigos HTTP adequados e mensagens claras em caso de erro, seguindo as melhores práticas de design de APIs REST.

## Como Rodar a Aplicação

### Pré-requisitos
Antes de executar o projeto, certifique-se de ter os seguintes requisitos instalados:
- **Java 17 ou superior**
- **Maven** para gerenciar dependências e construir o projeto
- **Spring Boot** para a configuração da aplicação
