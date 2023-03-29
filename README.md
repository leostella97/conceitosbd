# Conceitos de Banco de Dados

<ul>
	<a href="https://github.com/leostella97/conceitosbd#introdu%C3%A7%C3%A3o-ao-banco-de-dados"><b>Introdução</b></a>
	<li><a href="https://github.com/leostella97/conceitosbd#sistema-de-gerenciamento-de-banco-de-dados-sgbd">Sistema de Gerenciamento de Banco de Dados (SGBD)</a></li>
	<li><a href="https://github.com/leostella97/conceitosbd#modelagem-de-dados-para-banco-de-dados">Modelagem de Dados para Banco de Dados</a></li>
	<li><a href="https://github.com/leostella97/conceitosbd#arquitetura-para-banco-de-dados">Arquitetura para Banco de Dados
	<a href="">Modelo de Entidade Realcional (MER) com Banco de Dados</a>
	<li><a href="">Fundamentos de Modelagem e Projeto de Banco de Dados</a></li>
</a></li>
</ul>

<b>Banco de dados</b> é um <i>conjunto organizado</i> de informações que são armazenadas em um sistema de computador. Essas informações são <b>estruturadas</b> de tal forma que podem ser <i>facilmente acessadas, gerenciadas e atualizadas</i>.

Existem <b>vários tipos</b> de bancos de dados, sendo os mais comuns:

<b>• Banco de dados relacional:</b> é um tipo de banco de dados que <i>organiza as informações</i> em tabelas com linhas e colunas, sendo cada coluna representando um atributo dos dados e cada linha uma instância desses dados.
<br>
<b>• Banco de dados não relacional:</b> é um tipo de banco de dados que <i>não usa a estrutura de tabelas</i>, mas sim outros modelos de dados, como <i>documentos, grafos ou chave-valor</i>.
<b>• Banco de dados de objetos</b>: é um tipo de banco de dados que <i>armazena objetos</i> em vez de dados primitivos, permitindo uma maior flexibilidade na modelagem dos dados.
<b>• Banco de dados em memória</b>: é um tipo de banco de dados que <i>armazena os dados na memória principal</i> do computador, em vez de em um disco rígido, permitindo um <i>acesso muito mais rápido</i> aos dados.
<b>• Banco de dados distribuído</b>: é um tipo de banco de dados em que os dados <i>são armazenados</i> em vários computadores interconectados em rede, permitindo um processamento <i>mais rápido e distribuído</i> das informações.

## Introdução ao banco de dados
Como dito anteriormente, um <b>banco de dados</b> é uma <b>coleção organizada</b> de informações que podem ser facilmente <i>acessadas, gerenciadas e atualizadas</i> por meio de um sistema de computador. O objetivo principal do banco de dados é <b>permitir</b> que as informações sejam armazenadas de maneira estruturada, para que possam ser <i>recuperadas e utilizadas</i> com facilidade.

Existem <b>vários tipos</b> de bancos de dados, cada um com suas próprias <i>características e usos</i>. Um dos tipos mais comuns é o <b>banco de dados relacional</b>, que <i>organiza as informações em tabelas</i> com linhas e colunas. Cada coluna representa um <b>atributo dos dados</b> e cada linha uma <b>instância desses dados</b>. Outros tipos de bancos de dados incluem o banco de dados não relacional, o banco de dados de objetos, o banco de dados em memória e o banco de dados distribuído.

Os bancos de dados <b>são amplamente utilizados</b> em várias áreas, como <i>negócios, finanças, saúde, ciência e tecnologia</i>. Eles permitem que as empresas <b>armazenem e gerenciem</b> informações importantes, como dados do cliente, informações de vendas e estoque, além de ajudar no gerenciamento de recursos humanos e financeiros.

Um banco de dados é uma <b>ferramenta essencial</b> para armazenar e gerenciar informações importantes de forma organizada e acessível, facilitando o gerenciamento e a tomada de decisões de uma empresa.

## Sistema de Gerenciamento de Banco de Dados (SGBD)
O <b>sistema de gerenciamento de banco de dados (SGBD)</b> é um software projetado para <b>gerenciar e organizar</b> bancos de dados. Ele fornece uma interface para que os usuários possam <i>inserir, atualizar e recuperar</i> informações do banco de dados de maneira eficiente.

Existem vários tipos de SGBDs disponíveis, incluindo <b>SGBDs relacionais, NoSQL e orientados a objetos</b>;
<br>
<b>• SGBD relacional:</b> é o tipo mais comum e usa tabelas para armazenar dados relacionais;
<br>
<b>• NoSQL:</b>: por sua vez, é utilizado para <i>armazenar grandes quantidades</i> de dados não estruturados;
<br>
<b>• SGBD orientado a objetos:</b> é usado para armazenar objetos em vez de tabelas.

Um SGBD geralmente inclui um <b>conjunto de ferramentas</b> para gerenciar o banco de dados, como ferramentas para <i>criar, modificar e excluir</i> tabelas e índices. Ele também fornece mecanismos para controlar o acesso ao banco de dados, <i>garantindo a segurança e a integridade</i> dos dados.

Outras funções do SGBD incluem a execução de consultas complexas em grandes volumes de dados, gerenciamento de transações, controle de concorrência, backup e recuperação de dados e monitoramento de desempenho. A escolha do SGBD certo para uma determinada aplicação dependerá do tipo e volume de dados que precisam ser gerenciados, bem como das necessidades de segurança, escalabilidade e desempenho.

## Modelagem de Dados para Banco de Dados
No <b>contexto de banco de dados</b>, a <b>modelagem de dados</b> envolve a <i>criação de um modelo (podendo ser feito no <a href="draw.io">draw.io</a>) </i> que represente as informações que serão armazenadas no banco de dados. Esse modelo é <i>composto por entidades (tabelas), atributos (colunas) e relacionamentos entre as entidades</i>.

O objetivo da modelagem de dados é <b>garantir</b> que o banco de dados seja <i>eficiente, seguro e fácil de usar</i>. Um bom modelo de dados deve <b>refletir com precisão</b> a estrutura dos dados, além de <b>atender</b> aos requisitos de negócios e às necessidades dos usuários finais.

<i>Existem várias abordagens</i> para a modelagem de dados, como a abordagem <i>entidade-relacionamento (ER) e a abordagem orientada a objetos</i>. Cada uma dessas abordagens tem suas próprias técnicas e ferramentas de modelagem.

A modelagem de dados é uma <b>etapa importante</b> no desenvolvimento de um sistema de banco de dados e deve ser realizada com cuidado para <i>garantir a eficácia e a eficiência</i> do sistema de informação como um todo.

## Arquitetura para Banco de Dados
A arquitetura de um banco de dados refere-se à <b>estrutura e organização</b> dos componentes que permitem o <i>armazenamento, gerenciamento e recuperação de informações</i>. A arquitetura pode ser dividida em três camadas principais: <i>a camada física, a camada lógica e a camada de visão</i>.

A camada física <b>refere-se aos dispositivos físicos de armazenamento</b>, como discos rígidos, fitas magnéticas, unidades de estado sólido (SSDs) e outras tecnologias de armazenamento. Esses dispositivos são responsáveis por <i>armazenar os dados do banco de dados</i>.

A camada lógica inclui o software que <b>gerencia o acesso e a manipulação</b> dos dados armazenados na camada física. Isso inclui o <i>sistema de gerenciamento de banco de dados (SGBD)</i>, que fornece uma interface para que os usuários possam <i>interagir com os dados</i>. A camada lógica também inclui a linguagem de consulta estruturada (SQL) usada para <b>acessar e manipular</b> os dados.

A camada de visão <b>refere-se à interface</b> que permite que os usuários visualizem e interajam com os dados. Isso inclui aplicativos de software, páginas da web e outros meios pelos quais os usuários <i>podem acessar o banco de dados (por exemplo o PHPMyAdmin e o MySQL Workbench)</i>.

Uma arquitetura bem projetada pode <b>garantir</b> um <i>desempenho eficiente, segurança, integridade e disponibilidade</i> dos dados em um banco de dados.

# Modelo de Entidade Realcional (MER) com Banco de Dados

## Fundamentos de Modelagem e Projeto de Banco de Dados
A <b>modelagem e o projeto</b> de banco de dados são <b>fundamentais</b> para o <i>desenvolvimento de sistemas de informação</i> eficientes e confiáveis. Essas atividades envolvem a definição da estrutura dos dados que serão <i>armazenados, organizados e recuperados pelo sistema</i>.

A <b>modelagem de dados</b> é o processo de criação de um modelo conceitual que <i>descreve os objetos, entidades e relacionamentos</i> que serão representados no banco de dados. Essa etapa é importante para <b>definir a semântica</b> dos dados e <b>garantir</b> que as informações sejam <b>armazenadas de forma coerente</b>.

Já o <b>projeto de banco de dados</b> é a etapa em que o modelo conceitual é <i>transformado em um esquema lógico</i> que pode ser implementado em um <b>sistema de gerenciamento de banco de dados (SGDB)</b>. Nessa etapa, são definidos os <i>tipos de dados, as restrições de integridade e as estratégias de acesso e recuperação de dados</i>.

Um bom projeto de banco de dados <b>deve ser baseado</b> em uma análise cuidadosa dos requisitos do sistema e das necessidades dos usuários. Além disso, deve levar em consideração aspectos como <i>desempenho, escalabilidade, segurança e manutenibilidade do sistema</i>.

Por fim, é <b>importante</b> destacar que a modelagem e o projeto de banco de dados <i>são atividades contínuas e iterativas</i>. À medida que novos requisitos surgem ou que o sistema evolui, é necessário <b>atualizar e refinar</b> o modelo e o projeto para garantir a <i>eficiência e a confiabilidade do sistema</i>.