<p align="center">
  <img width="500" height="500" src="https://desafiodocodigo.com.br/desafio/img/desafiodocodigo-pb.png">
</p>

## O que é?

O "[Desafio do Código](http://desafiodocodigo.com.br)" é um desafio online com um conjunto de missões que guiam você por ferramentas digitais para aprender programação, matemática e inglês. 
Foi criado por [Soraia Novaes](http://professoragoogle.com.br/) para auxiliar crianças de 10 a 108 anos a aprender estas habilidades tão necessárias no mundo atual.

## Este repositório

É o repositório único do projeto no qual estamos trabalhando em uma **nova versão** com um padrão **mais limpo e moderno de código** a partir da iniciativa de [Tiago Gouvêa](http://www.tiagogouvea.com.br). 

O código antigo foi implementado em PHP por alguns voluntários e está na branch [desafioAntigo](/https://github.com/TiagoGouvea/desafio_do_codigo/tree/desafioAntigo). 

Tudo por aqui está (e deverá continuar) em português, incluíndo comentários em códigos, para permitir que mais pessoas contribuam com o projeto.

# Contribuindo

Ficaremos muitos felizes em ver você contribuindo conosco! Se esse é seu desejo dê uma lida em "[Como Contribuir](CONTRIBUTING.md)".

# Componentes e estrutura do projeto

Optamos por usar frameworks mais simples, para que jovens e estudantes possam trabalhar bem com o projeto. Estamos usando: 

* PHP 7 - Para que tudo funcione como esperado
* [Composer](https://getcomposer.org) - Gerenciador de dependências 
* [Slim Framework](https://www.slimframework.com/) - É quem carrega a base do projeto, define as rotas e lida com as requisições
* [Twig](https://twig.symfony.com) - É o responsável por renderizar as views, mesclar os dados fornecidos pelo PHP com o HTML
* [Bootstrap](https://getbootstrap.com/) - Para manter as views fáceis de serem construídas e sempre responsivas

A estrutura de pastas do projeto segue o padrão do Slim, com poucas modificações:

```
/
|--- app/
|      |--- src/
|      |      |--- Controller
|      |      |--- Model
|      |      |--- Middleware
|      |      |--- Persistence
|      |      |--- View/
|      |--- dependencies.php
|      |--- routes.php
|      |--- settings.php
|--- public/
|      |--- css/
|      |--- js/
|      |--- index.php
```

Certamente em 99% do tempo você estará trabalhando nos arquivos das pastas **Controller**, **Model**, **View** e **public**. 

# Rodando o projeto novo em desenvolvimento

1. Baixe o código do repositório usando seu git;
1. Acesse a pasta do projeto e execute ``php composer.phar install`` para instalar as dependências;
1. Dê seu navegado, acesse seu localhost, algo como ``http://localhost/desafio_do_codigo/public/``. Você verá as instruções para concluir sua configuração;
1. Crie um arquivo settings.php em /app/, usando como base o settings.template.php

* Será necessário ter permissão de escrita na pasta /cache/. Se você usa Mac ou Linux precisará dar esta permissão pelo terminal.

Tudo pronto para programar! :D

