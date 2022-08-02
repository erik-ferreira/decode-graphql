# GraphQL

QL - Query Language
Objetivo - Server para realizar operações de escrita e leitura através da comunicação do front com o back

- Quais problemas GraphQL resolve?

  - Overfetching - Buscar informações demais

    - http://localhost:3000/users
      - DB (usuários, endereços)

  - Underfetching - Buscar poucas informações
    - http://localhost:3000/users
      - DB (usuários)

- Dificuldades
  - Cache
  - Erros

```gql
query {
  users {
    id
    name
    github

    addresses {
      city
      state
      country
    }
  }
}
```

## Backend com GraphQL

Possuí duas estratégias:

- schema first
- code first [x]

## Code First

1. yarn add type-graphql graphql apollo-server class-validator reflect-metadata
2. yarn add typescript @types/node ts-node-dev -D
3. Dois conceitos do GraphQL:
4. query: buscar dados
5. mutation: criar, alterar ou deletar dados

<!-- 00:53:00 -->
