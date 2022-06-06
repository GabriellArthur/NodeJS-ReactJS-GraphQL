O front-end se responsabiliza pelas querys que o back-end deve fazer.

# Quais problemas GraphQl resolve?

- Overfetching
    - Buscar informações de mais, realizar o "fetching" a mais que eu preciso
    - http://localhost:3000/users
        - BD (usuários, endereços)
    - http://localhost:3000/users
        - BD (usuários)
- Underfetching 
    - Buscar dados de menos
    - http://localhost:3000/users
        - BD (usuários)
    - http://localhost:3000/addresses

# Dificuldades

- Complexidade
- Cache
- Erros


// http://localhost:3000/graphql

# Exemplo no front-end

```gql
query {
    users {
        id,
        name,
        github,
        addresses {
            city,
            state,
            country,
        },
    }
}
```

