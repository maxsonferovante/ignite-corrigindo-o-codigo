Claro, vou colocar tudo em um único bloco de markdown para facilitar a inclusão no README:


<h1 align="center">Desafio 03 - Corrigindo o Código</h1>


<p align="center">
  <img alt="Rocketseat Education" src="https://avatars.githubusercontent.com/u/69590972?s=200&v=4" width="100px" />
</p>

<p align="center">
  <img src="https://img.shields.io/static/v1?label=Rocketseat&message=Education&color=8257e5&labelColor=202024" alt="Rocketseat Project" />
  <a href="LICENSE"><img  src="https://img.shields.io/static/v1?label=License&message=MIT&color=8257e5&labelColor=202024" alt="License"></a>
</p>

## 🚀 O que é e o propósito do projeto

Este projeto é parte do Desafio 03 do Bootcamp Ignite da Rocketseat, que se concentra em corrigir uma aplicação Node.js que gerencia repositórios de projetos e permite a adição de likes a esses repositórios. Alguns testes não estão passando após alterações no código, e a missão é corrigi-lo para garantir o funcionamento correto.

A aplicação lida com operações de CRUD (Create, Read, Update, Delete) para repositórios, permitindo a adição, listagem, atualização e exclusão deles. Além disso, é possível adicionar likes a esses repositórios.


A aplicação segue a seguinte estrutura para um novo repositório:
```jsx
{
  id: uuid(),
  title,
  url,
  techs,
  likes: 0
}
```

## 💻 Tecnologias

- [Node.js](https://nodejs.org/)
- [Express](https://expressjs.com/)
- [UUID](https://github.com/uuidjs/uuid)
- ...

## 🔧 Especificação dos Testes

Os testes validam o correto funcionamento das funcionalidades da aplicação, incluindo a criação de novos repositórios, listagem, atualização, exclusão e adição de likes.

## 🔌 Middlewares da aplicação

Neste desafio, o foco é nos middlewares, que desempenham funções cruciais para garantir o funcionamento correto da aplicação. Aqui está uma breve descrição de cada middleware:

### checksExistsUserAccount

Valida a existência de um usuário com base no `username` passado no header da requisição. Se existir, repassa o usuário para `request.user` e chama a função `next`.

### checksCreateTodosUserAvailability

Verifica se o usuário pode criar um novo *todo* com base no plano (grátis ou Pro) e na quantidade de *todos* que possui. Permite a criação se estiver no plano grátis e tiver menos de 10 *todos* ou se estiver no plano Pro.

### checksTodoExists

Valida se o *todo* pertence ao usuário, com base no `username` do header e no `id` do *todo* passado nos parâmetros. Se válido, passa o *todo* e o usuário para `request.todo` e `request.user`, respectivamente, e chama a função `next`.

### findUserById

Localiza um usuário com base no `id` fornecido nos parâmetros da rota. Se encontrado, repassa o usuário para `request.user` e chama a função `next`.

## 🛠️ Como usar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/desafio-03-corrigindo-o-codigo.git
   ```

2. Acesse o diretório do projeto:
   ```bash
   cd desafio-03-corrigindo-o-codigo
   ```

3. Instale as dependências:
   ```bash
   yarn install
   ```

4. Execute os testes:
   ```bash
   yarn test
   ```

   Certifique-se de que os testes foram bem-sucedidos, e se não foram, faça as correções necessárias no código.

5. Para iniciar a aplicação:
   ```bash
   yarn start
   ```

   A aplicação estará disponível em http://localhost:3333.

---

## 📝 Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.


Feito com 💜 por Maxson Almeida 👋

[GitHub](https://github.com/maxsonferovante)
[LinkedIn](https://www.linkedin.com/in/maxson-almeida-501065260/)
```