# Loja de Carros - API README

Bem-vindo ao projeto **Loja de Carros**, uma API Node.js que gerencia informações sobre carros e usuários, utilizando autenticação com criptografia. Neste projeto, foi utilizado o framework **Express** para construir a API e o banco de dados **PostgreSQL** para armazenar os dados. Além disso, a autenticação dos usuários é feita por meio do uso de tokens **JWT** (JSON Web Tokens) para garantir a segurança das informações.

## Tecnologias Utilizadas

- Node.js
- Express.js
- PostgreSQL
- bcrypt
- jsonwebtoken

## Estrutura do Projeto

### `carros.js`

Este módulo contém as funções para manipulação de dados relacionados a carros, como listagem, detalhamento, cadastro, atualização e exclusão.

### `usuarios.js`

Neste módulo, estão as funções relacionadas aos usuários, incluindo cadastro, login e obtenção de perfil.

### `autenticacao.js`

Módulo responsável por verificar a autenticação do usuário antes de permitir o acesso a determinadas rotas.

### `conexao.js`

Aqui está a configuração da conexão com o banco de dados PostgreSQL.

### `index.js`

O ponto de entrada da aplicação, onde são configurados os middlewares e as rotas.

### `rotas.js`

Definição das rotas da API:

- `POST /usuario`: Cadastrar um novo usuário.
- `POST /login`: Realizar login e receber um token JWT.
- `GET /perfil`: Obter o perfil do usuário autenticado.
- `GET /carro`: Listar todos os carros.
- `GET /carro/:id`: Detalhar informações de um carro específico.
- `POST /carro`: Cadastrar um novo carro.
- `PUT /carro/:id`: Atualizar informações de um carro.
- `DELETE /carro/:id`: Excluir um carro.

### Configuração e Uso

1. Instale as dependências do projeto:

   ```bash
   npm install
   
Certifique-se de que o PostgreSQL esteja instalado e configurado. 

Crie um banco de dados com o nome loja_carros_autenticacao_criptografia e execute o script dump.sql para criar as tabelas necessárias.

Configure as variáveis de ambiente no arquivo .env (não fornecido no código fornecido, mas uma boa prática em um ambiente de produção real) para armazenar informações sensíveis, como chaves secretas e informações de conexão com o banco de dados.

Inicie o servidor:

`npm run dev`

### Considerações Finais


Este projeto é uma demonstração de como construir uma API utilizando Node.js, Express.js e PostgreSQL, com foco em autenticação e segurança. 

Certifique-se de entender e ajustar as configurações de segurança e autenticação para atender às necessidades do seu ambiente de produção.

Sinta-se à vontade para explorar, modificar e expandir este projeto de acordo com suas necessidades. Em caso de dúvidas ou sugestões, não hesite em entrar em contato!

Divirta-se codificando! 😄🚗🔐🎉
