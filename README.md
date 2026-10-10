# Baozi Store — API REST

Projeto acadêmico de Desenvolvimento Web Back-End. Implementado com Java 17, Spring Boot, Spring Data JPA e banco relacional H2 em arquivo.

## Requisitos
- Java 17+
- Maven 3.8+ (ou Maven Wrapper criado pela IDE)

## Executar
1. Abra a pasta do projeto no IntelliJ IDEA, Eclipse ou VS Code com suporte a Java.
2. Execute `mvn spring-boot:run` na pasta que contém `pom.xml`.
3. A API ficará disponível em `http://localhost:8080`.

## Endpoints
| Método | Caminho | Ação |
|---|---|---|
| POST | `/api/clientes` | Criar cliente |
| GET | `/api/clientes` | Listar clientes |
| GET | `/api/clientes/{id}` | Consultar cliente |
| DELETE | `/api/clientes/{id}` | Excluir cliente |
| POST | `/api/produtos` | Criar produto |
| GET | `/api/produtos` | Listar produtos |
| GET | `/api/produtos/{id}` | Consultar produto |
| DELETE | `/api/produtos/{id}` | Excluir produto |
| POST | `/api/pedidos` | Criar pedido |
| GET | `/api/pedidos` | Listar pedidos |
| GET | `/api/pedidos/{id}` | Consultar pedido |
| DELETE | `/api/pedidos/{id}` | Excluir pedido |

## Exemplos de JSON para Postman

Cliente:
```json
{"nome":"Gabriel5263613","clienteDesde":"2026-10-09"}
```

Produto:
```json
{"nome":"Baozi tradicional","preco":8.50,"estoque":true}
```

Pedido (substitua os IDs pelos retornados pela API):
```json
{"clienteId":1,"produtoId":1,"quantidade":3}
```

No Postman, use `http://localhost:8080` como base URL e `Content-Type: application/json` para requisições POST.

## Observação acadêmica
Os prints do Postman e o link do repositório devem ser adicionados após executar e testar o projeto. Não inclua capturas fictícias como se fossem testes reais.
