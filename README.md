<div id='top' align="center">

  # Challenge Backend: AdoPet

  > A **AdoPet 🐾** é uma empresa fictícia que funciona como intermediária entre pessoas que querem adotar pets e ONGs recolhem os animais das ruas.  

  <a>Potuguese</a> -
  <a href="./docs/en/README_en.md">English</a>

</div>

<div id='tech'>

  ## 🤖 Tecnologias usadas

</div>
<div align="center">
  <a href='https://nodejs.org/' target='_blank'><img src="https://img.shields.io/badge/Node.js-white?style=for-the-badge&logo=node.js&logoColor=green">
  <a href='https://react.dev/' target='_blank'><img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
  <a href='https://expressjs.com/' target='_blank'><img src="https://img.shields.io/badge/Express-1572B6?style=for-the-badge&logo=express&logoColor=white">
  <a href='https://jwt.io/' target='_blank'><img src="https://img.shields.io/badge/JWT-61B?style=for-the-badge&logo=jsonwebtokens&logoColor=white"/></a>
  <a href='https://www.postgresql.org/' target='_blank'><img src="https://img.shields.io/badge/PostgreSQL-F6F5F2?style=for-the-badge&logo=postgresql&logoColor=blue"/></a>
  <a href='https://sequelize.org/' target='_blank'><img src="https://img.shields.io/badge/Sequelize-52B0E7?style=for-the-badge&logo=sequelize&logoColor=white"/></a>
  <a href='https://www.cypress.io/' target='_blank'><img src="https://img.shields.io/badge/Cypress-69D3A7?style=for-the-badge&logo=Cypress&logoColor=white"/></a>
  <a href='https://jestjs.io/' target='_blank'><img src="https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white"/></a>
  <a href='https://www.docker.com/' target='_blank'><img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/></a>
  <a href='https://render.com/' target='_blank'><img src="https://img.shields.io/badge/Render-46E3B7?style=for-the-badge&logo=render&logoColor=white"/></a>
  <a href='https://nodemon.io/' target='_blank'><img src="https://img.shields.io/badge/Nodemon-76D04B?style=for-the-badge&logo=nodemon&logoColor=white"/></a>
  <a href='https://docs.github.com/en/actions' target='_blank'><img src="https://img.shields.io/badge/GitHub Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white"/></a>
  <a href='https://fakerjs.dev/' target='_blank'><img src="https://img.shields.io/badge/Faker-  06C167?style=for-the-badge&logoColor=white"/></a>
</div>


## 🦾 Sobre o desafio

Este projeto foi desenvolvido como resultado de um Desafio Back-End exclusivo para alunos da escola de tecnologia [Alura](https://www.alura.com.br).

O desafio consiste em simular um ambiente de trabalho real no qual é disponibilizado tarefas através do Trello com entregas semanais, durante 4 semanas. Cada tarefa descreve o que o cliente fictício deseja que seja construído. Temos a liberdade de realizar modificações ou seguir novas abordagens a depender das necessidades e criatividade. Podemos também escolher as tecnologias que desejarmos para desenvolver o projeto. 


## 👨🏽‍💻 Sobre o desenvolvimento

No desenvolvido da API foi utilizado o [Express](https://expressjs.com/) como framework de construção de aplicações web, o ORM [Sequelize]() para abstrair a integração com o banco de dados SQL entre outras tecnologias listadas <a href='#tech'>☝🏾 logo acima</a>, todos como forma de praticar os conceitos das bibliotecas, ferramentas e construção de APIs RESTful.

Para a integração da API com o Front-End previamente desponibilizado, explorei os recursos do [React](https://react.dev/) para realizar as chamadas da API com o **UseEffect**, organizar o código da autenticação via login através dos **hooks** e **contexts**, entre outros recursos que foram sendo necessários durante os ajustes no desenvolvimento e testes. 

A API abrange rotas para gerenciamento de usuários, pets, abrigos, perfil e permissões. Assim como autenticação de usuários através de login e autorização de acesso as rotas por meio de tokens JWT gererado no login. Além disso, há também o controle via permissão às rotas por perfil de usuário. 

Para os _testes de unidade_ e _integração_ na **API** foi usado [Jest](https://jestjs.io), enquanto para os _testes E2E_ no **Front-end** foi usado o [Cypress](https://www.cypress.io/) como test runner.

Usei o [Docker](https://www.docker.com/) para a construção da imagem e o [Docker Compose](https://docs.docker.com/compose/) para subir a aplicação e o banco de dados localmente para dar suporte ao desenvolvimento e testes. 

Há testes e build automatizados que são realizados pelo [GithHub Actions](https://docs.github.com/en/actions) toda vez que um novo commit é enviado para branch principal do repositório da API. Uma vez que todas as verificação são validadas é gerada uma imagem docker e publicada no [Docker Hub](https://hub.docker.com/repository/docker/jeffersonps/adopet-api/general).

O deploy da API e do Front-End é realizado pela plataforma do [Render](https://render.com/), também de forma automática seguindo a mesma regra descrito acima.

Contudo uma refatoração futura do código será necessária após a evolução dos meus estudos.

- 🚀 [Acesse o site](https://adopet.sapituca.site/) para conhecer o **AdoPet**.

<a href='https://adopet.sapituca.site/' target='_blank'><img src="./docs/assets/adopet.png"/></a>

<div id="projects">

## 🏗️ Projetos
- 🚀 [AdoPet API](https://github.com/jeff-pedro/adopet-api)
- 🐾 [AdoPet site](https://github.com/jeff-pedro/adopet-client)

</div>


## ⚙️ Como usar esse repositório

Este repositório consiste de dois **módulos**, a api e o front-end do Adopet.
É possivels clonar os [projetos](#projects) individualmente ou através deste repositório via **[git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules).**

Clone este repositório atualizando recursivamente os módulos
```shell
git clone --recurse-submodules https://github.com/jeff-pedro/challenge-backend-adopet.git
```

E leia os READMEs de cadas [projeto](#projects) para aprender como usuá-los.

---

<a href='#top'>☝🏾 Voltar ao topo</a>
