# Ignite - Desafio 02 - Trabalhando com middlewares
Nesse desafio você irá trabalhar mais a fundo com middlewares no Express. Dessa forma você será capaz de fixar mais ainda os conhecimentos obtidos até agora. 

Para facilitar um pouco mais do conhecimento da regra de negócio, você irá trabalhar com a mesma aplicação do desafio anterior: uma aplicação para gerenciar tarefas (ou *todos*) mas com algumas mudanças.

Será permitida a criação de um usuário com `name` e `username`, bem como fazer o CRUD de *todos*:

- Criar um novo *todo*;
- Listar todos os *todos*;
- Alterar o `title` e `deadline` de um *todo* existente;
- Marcar um *todo* como feito;
- Excluir um *todo*;

Tudo isso para cada usuário em específico. Além disso, dessa vez teremos um plano grátis onde o usuário só pode criar até dez *todos* e um plano Pro que irá permitir criar *todos* ilimitados, isso tudo usando middlewares para fazer as validações necessárias.

## Especificação dos Testes de Middlewares

- [x] Deve ser possível encontrar um usuário pelo nome de usuário e passar através do `request.user`

- [x] Não deve ser possível encontrar um usuário com nome de usuário inexistente.

- [x] Deve ser possível criar uma nova tarefa quando o usuário possui  menos de dez tarefas cadastradas.

- [x] Não deve ser possível criar uma nova tarefa quando o usuário não possuir o plano Pró e já tiver dez tarefas cadastradas.

- [x] Deve ser possível criar infinitas tarefas quando o usuário possuir plano Pró.

- [x] Deve ser possível passar o usuário e a tarefa, através do request quando ambos existirem.

- [x] Não deve ser possível repassar usuário pelo request quando usuário for inexistente.

- [x] Não deve ser possível repassar usuário e tarefa pelo request quando o id não for uuid.

- [x] Não deve ser possível repassar usuário e tarefa pelo request quando a tarefa for inexistente.

- [x] Deve ser possível encontrar um usuário pelo id informado como parâmetro da rota e repassar o mesmo pelo `request.user`.

- [x] Não deve ser possível repassar o usuário pelo `request.user` quando o usuário for inexistente para o id informado.


## Executando a aplicação

- Após clonar o repositório, navegue até o diretório pelo terminal e execute o comando `yarn` para instalar todas as dependências.

- Execute o comando `yarn dev` para rodar a aplicação em modo de desenvolvimento

- Execute o comando `yarn test` para rodar os testes.