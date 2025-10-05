# Image-Uploader

API para upload, listagem, atualização e remoção de imagens usando Node.js, Express e MySQL.

## Instalação

```sh
npm install
```

## Configuração

Crie um arquivo `.env` com:

```
PORT=3000
MYSQL_HOST=localhost
MYSQL_USER=seu_usuario
MYSQL_PASSWORD=sua_senha
MYSQL_DB=aula_upload
```

## Banco de Dados

Crie o banco e a tabela:

```sql
CREATE DATABASE aula_upload;
USE aula_upload;
CREATE TABLE images (
  id INT AUTO_INCREMENT PRIMARY KEY,
  img VARCHAR(255) NOT NULL
);
```

## Uso

```sh
npm run dev
```

## Rotas

- `POST /api/images` (form-data, key: image)
- `GET /api/images`
- `PUT /api/images/:id` (form-data, key: image)
- `DELETE /api/images/:id`
