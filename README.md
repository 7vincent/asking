<p align="center">
  <img src="logo.svg" height="150" width="175" alt="Asking" />
</p>

<h3 align="center">
  Interaja com seu público em suas palestras! 🚀
</h3>

<br>

<div align="center">

<h1><b>ASKING</b></h1>

</div>
## Overview

Sistema para auxiliar na interação do público com o palestrante através de perguntas.

## Para rodar o projeto

#### API
Ao clonar esse repositório para sua maquina, descompacte, entre na pasta asking-api e abra o terminal nesta pasta.

No terminal insira os seguintes comandos:

1. Digite `yarn` para carregar as dependências.
2. Digite `docker-compose up -d` para construir e iniciar um container Docker para criação do banco Postgres. 
3. Agora dê um `yarn dev` para criação das tabelas e inicio da execução da api.
4. Em outro terminal, digite: `yarn sequelize db:seed:all` para criação de um user padrão, que lhe dará acesso a aplicação.
5. Após a execução dos passos acima, você vai ter a api rodando com um user criado.

### APP

Da mesma forma que a api, ao clonar esse repositório para sua maquina, descompacte, entre na pasta asking-app e abra o terminal nesta pasta.

1. No terminal insira o seguinte comandos: `yarn start`
2. Ao abrir a pagina de login faça login com os seguintes dados:
User: root@admin.com
Pass: 123456

## Funcionalidades da aplicação:

### Criação de avento
1. click no "+" para criar um evento;
2. Insira os dados nos campos e click em enviar;
3. Volte para a lista de eventos;
4. Click no evento criado anteriormente;
5. Vai abrir a pagina das perguntas do evento, habilite o evento clicando no botão vende (icone de play);

A partir de agora, qualquer um que acessar, no nosso caso de teste, uma janela anônima http://localhost:3333/duvida vai cair no formulario para fazer uma pergunta ao evento em questão;

### Fazendo perguntas

1. Abra outra janela anônima para simular o que seria a janela que vai ficar no telão da palestra e acesse: http://localhost:3333;

2. Com as 3 janelas abertas, vá no form de dúvida (http://localhost:3333/duvida) e cadastre uma nova pergunta;

3. Automaticamente a janela que vc estará logado, que criou o evento, vai aparecer a pergunta inserida, com 2 botões, um para arquivar e outro para mandar para o telão;

### Habilitanto perguntas no telão

Clique em enviar para o telão e veja a janela anônima que estaria no telão sendo atualizada com a pergunta; 

## Tecnologias envolvidas no Projeto
1. Node.js
2. React.js
3. Docker
4. Postgres
