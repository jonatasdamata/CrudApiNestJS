# API de Controle de Desenvolvedores
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/jonatasdamata/CrudApiNestJS/blob/main/LICENSE) 


## Descrição
Uma API CRUD desenvolvida com **NestJS** para gerenciar informações de desenvolvedores. Esta API permite realizar operações de listagem, criação, atualização e exclusão de desenvolvedores, seguindo as melhores práticas de desenvolvimento de APIs RESTful.


## Funcionalidades

- **Listar Desenvolvedores**: Obtém uma lista de todos os desenvolvedores.
- **Obter Desenvolvedor por ID**: Permite buscar um desenvolvedor específico usando seu ID.
- **Criar Novo Desenvolvedor**: Adiciona um novo desenvolvedor ao sistema.
- **Atualizar Desenvolvedor**: Atualiza informações de um desenvolvedor existente.
- **Excluir Desenvolvedor**: Remove um desenvolvedor do sistema.
- 

## Tecnologias Utilizadas

- **Node.js**
- **NestJS**
- **TypeScript**
- **TypeORM** 
- **Postman** 



## Como Executar o Projeto

### Pré-requisitos

1. Certifique-se de ter o [Node.js](https://nodejs.org/) instalado.
2. Certifique-se de ter o [npm](https://www.npmjs.com/) instalado (geralmente já vem com o Node.js).
3. Execute o seguinte comando para instalar as dependências do projeto:

```bash
npm install sqlite3 nanoid reflect-metadata rxjs class-transformer class-validator typeorm
````


## Executando a Aplicação

### Clone este repositório:
```bash
git clone https://github.com/jonatasdamata/CrudApiNestJS
```

### Navegue até o diretório do projeto:
```bash
cd CrudApiNestJS
```
A API estará disponível em http://localhost:3000


## Endpoints da API

| Método | Endpoint               | Descrição                             |
|--------|------------------------|---------------------------------------|
| GET    | /developers            | Lista todos os desenvolvedores        |
| GET    | /developers/{id}       | Obtém um desenvolvedor pelo ID        |
| POST   | /developers            | Cria um novo desenvolvedor            |
| PATCH  | /developers/{id}       | Atualiza um desenvolvedor existente   |
| DELETE | /developers/{id}       | Remove um desenvolvedor               |


## Exemplos de Uso

### Listar Desenvolvedores
```http
GET http://localhost:3000/developers
```
### Obter Desenvolvedor
```http
GET http://localhost:3000/developers/{id}
```

### Criar Desenvolvedor
```http
POST http://localhost:3000/developers
Content-Type: application/json

{
    "name": "Maria",
    "email": "maria@teste.com",
    "dateOfBirth": "1996-02-10"
}
```

### Atualizar Desenvolvedor
```http
PATCH http://localhost:3000/developers/3
Content-Type: application/json

{
    "email": "jhon@teste.com"
}
```

### Deletar Desenvolvedor
```http
DELETE http://localhost:3000/developers/dev_DzITx-bXu_6IgXYWqoVrs
```




## Autor

Jonatas da Mata <br>
https://www.linkedin.com/in/jonatasdamata/
