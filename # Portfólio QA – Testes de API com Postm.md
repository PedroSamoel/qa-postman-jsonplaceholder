# Portfólio QA – Testes de API com Postman (JSONPlaceholder)

Este projeto demonstra testes de API automatizados usando o Postman e a API pública [JSONPlaceholder](https://jsonplaceholder.typicode.com).

## 📌 O que foi feito
- CRUD completo em **/users** e **/posts**
- Validação de status code, formato JSON e tempo de resposta
- Testes automáticos de campos obrigatórios (id, name, email)
- Encadeamento de variáveis (userId, postId, commentId)
- Exemplos salvos (200, 201, 404) para documentação

## 🚀 Como usar no Postman
1. Baixe os arquivos da pasta `collections/` e `environments/`.
2. Importe no Postman:
   - Collection: `JSONPlaceholder.postman_collection.json`
   - Environment: `DEV-JSONPlaceholder.postman_environment.json`
3. Selecione o Environment no topo do Postman.
4. Execute as requisições na ordem CRUD.

## 📊 Relatórios (opcional com Newman)
Execute no terminal:
```bash
newman run collections/JSONPlaceholder.postman_collection.json \
  -e environments/DEV-JSONPlaceholder.postman_environment.json -r cli,html
