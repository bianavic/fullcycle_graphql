# fullcycle_graphql

---

## expondo aplicacao com graphql
site: https://gqlgen.com/

---

Estrutura graphql criada com gqlgen

## Inicia

```bash
go mod init github.com/bianavic/fullcycle_graphql 
```

## Instala Tools

```bash
 printf '//go:build tools\npackage tools\nimport (_ "github.com/99designs/gqlgen"\n _ "github.com/99designs/gqlgen/graphql/introspection")' | gofmt > tools.go
```

## Baixa pacotes

```bash
 go mod tidy
```

## Inicia gqlgen config e gera esquelto do projeto

```bash
go run github.com/99designs/gqlgen init
```

## Inicia server

```bash
go run server.go
```

## Acessa GraphQL Playground

```bash
http://localhost:8080/
```

OBS:
- Criar arquivo schema.graphqls
- Rodar comando go run github.com/99designs/gqlgen generate
- Executa resolver para implementar os metodos
- Rodar comando go run server.go
- Acessar http://localhost:8080/ para testar
OBS: O playground irá apresentar `Mutation` e `Query`