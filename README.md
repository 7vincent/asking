<p align="center">
  <img src="logo.svg" height="150" width="175" alt="Asking" />
</p>

<h3 align="center">
  Interaja com seu público em suas palestras! 🚀
</h3>

<br>

<div align="center">

[![Coverage Status](https://img.shields.io/coveralls/github/Rocketseat/unform.svg?color=%237159c1)](https://coveralls.io/github/Rocketseat/unform?branch=master)

</div>
# ASKING

## Overview

Sistema para auxiliar na interação do público com o palestrante através de perguntas.

## Para rodar o projeto

#### API
Ao clonar esse repositório para sua maquina, descompacte, entre na pasta asking-api e abra o terminal nesta pasta.

No terminal insira os seguintes comandos:

1. Digite `yarn` para carregar as dependências.
2. Digite `docker-compose up -d` para construir e iniciar um container Docker para criação do banco Postgres. 
3. Agora dÊ um `yarn dev` para criação das tabelas e inicio da execução da api.
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
click no "+" para criar um evento;
Insira os dados nos campos e click em enviar;
Volte para a lista de eventos;
Click no evento criado anteriormente;
Vai abrir a pagina das perguntas do evento, habilite o evento clicando no botão vende (icone de play);

A partir de agora, qualquer um que acessar, no nosso caso de teste, uma janela anônima http://localhost:3333/duvida vai cair no formulario para fazer uma pergunta ao evento em questão;

Abra outra janela anônima para simular o que seria a janela que vai ficar no telão da palestra e acesse: http://localhost:3333;

Com as 3 janelas abertas, vá no form de dúvida (http://localhost:3333/duvida) e cadastre uma nova pergunta;

Automaticamente a janela que vc estará logado, que criou o evento, vai aparecer a pergunta inserida, com 2 botões, um para arquivar e outro para mandar para o telão;

Clique em enviar para o telão e veja a janela anonima que estaria no telão sendo atualizada com a pergunta; 
