# Conceitos de Banco de Dados

<ul>
	<a href="https://github.com/leostella97/conceitosbd#introdu%C3%A7%C3%A3o-ao-banco-de-dados"><b>Introdução</b></a>
	<li><a href="https://github.com/leostella97/conceitosbd#sistema-de-gerenciamento-de-banco-de-dados-sgbd">Sistema de Gerenciamento de Banco de Dados (SGBD)</a></li>
	<li><a href="https://github.com/leostella97/conceitosbd#modelagem-de-dados-para-banco-de-dados">Modelagem de Dados para Banco de Dados</a></li>
	<li><a href="https://github.com/leostella97/conceitosbd#arquitetura-para-banco-de-dados">Arquitetura para Banco de Dados</a></li>
	<a href="https://github.com/leostella97/conceitosbd#modelo-de-entidade-realcional-mer-com-banco-de-dados"><b>Modelo de Entidade Realcional (MER) com Banco de Dados</b></a>
	<li><a href="https://github.com/leostella97/conceitosbd#fundamentos-de-modelagem-e-projeto-de-banco-de-dados">Fundamentos de Modelagem e Projeto de Banco de Dados</a></li>
	<li><a href="https://github.com/leostella97/conceitosbd#modelo-de-entidade-relacionamento-com-banco-de-dados">Modelo de Entidade Relacionamento com Banco de Dados</a></li>
	<li><a href="https://github.com/leostella97/conceitosbd#modelo-de-relacionamento-de-entidade-aprimorado-com-banco-de-dados">Modelo de Relacionamento de Entidade Aprimorado com Banco de Dados</a></li>
	<a href=""><b>Explorando a Linguagem de Consulta a Banco de Dados SQL</b></a>
	<li><a href="">Modelo Relacional e Mapeamento Relacional com Banco de Dados</a></li>
	<li><a href="https://github.com/leostella97/conceitosbd#primeiros-passos-com-sql">Primeiros Passos com SQL</a></li>
	<a href="https://github.com/leostella97/conceitosbd#explorando-queries-com-sql"><b>Explorando Queries com SQL</b></a>
	<li><a href="https://github.com/leostella97/conceitosbd#comandos-baseados-em-opera%C3%A7%C3%B5es-matem%C3%A1ticas-union-intersection-e-except">Comandos Baseados em Operações Matemáticas: UNION, INTERSECTION e EXCEPT</a></li>
	<li><a href="https://github.com/leostella97/conceitosbd#elaborando-queries-sql-com-express%C3%B5es">Elaborando Queries SQL com Expressões</a></li>
	<a href="https://github.com/leostella97/conceitosbd#criando-queries-com-fun%C3%A7%C3%B5es-e-cl%C3%A1usulas-de-agrupamentos"><b>Criando Queries com Funções e Cláusulas de Agrupamentos</b></a>
	<li><a href="https://github.com/leostella97/conceitosbd#order-by-cl%C3%A1usulas-de-ordena%C3%A7%C3%A3o-com-sql">ORDER BY: Cláusulas de ordenação com SQL</a></li>
	<li><a href="https://github.com/leostella97/conceitosbd#group-by-cl%C3%A1usulas-de-ordena%C3%A7%C3%A3o-com-sql">GROUP BY: Cláusulas de ordenação com SQL</a></li>
	<li><a href="https://github.com/leostella97/conceitosbd#having-statment">Having Statment</a></li>
	<a href="https://github.com/leostella97/conceitosbd#agrupamendo-registros-e-tabelas-com-join-statment"><b>Agrupamendo Registros e Tabelas com Join Statment</b></a>
	<li><a href="https://github.com/leostella97/conceitosbd#case-statment">CASE Statment</a></li>
	<li><a href="https://github.com/leostella97/conceitosbd#o-caso-zeronull-trick">O Caso Zero/Null Trick</a></li>
	<a href="https://github.com/leostella97/conceitosbd#personalizando-acessos-com-views"><b>Personalizando Acessos com Views</b></a>
	<li><a href="https://github.com/leostella97/conceitosbd#overview-sobre-automa%C3%A7%C3%A3o-de-a%C3%A7%C3%B5es-com-triggers-no-mysql">Overview sobre Automação de Ações com Triggers no MySQL</a></li>
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

### Características de um Banco de Dados
Um banco de dados é um <b>conjunto organizado</b> de dados que são <i>armazenados e gerenciados</i> em um sistema computacional. Algumas <b>características</b> de um banco de dados são:

<b>• Estrutura organizada:</b> os dados são organizados de uma forma estruturada, geralmente em tabelas, para facilitar a <i>busca, classificação e acesso às informações</i>.

<b>• Relacionamentos:</b> os dados podem estar relacionados entre si, permitindo a realização de consultas complexas que envolvem múltiplas tabelas.

<b>• Confiabilidade:</b> os bancos de dados são projetados para serem <b>confiáveis e duráveis</b>, protegendo os dados contra perda ou corrupção.

<b>• Controle de acesso:</b> os bancos de dados oferecem mecanismos de controle de acesso que permitem determinar quais usuários têm acesso a quais dados.

<b>• Consistência:</b> os bancos de dados são projetados para <b>manter a consistência</b> dos dados, mesmo que ocorram falhas no sistema.

<b>Escalabilidade:</b> os bancos de dados são projetados para suportar grandes quantidades de dados e muitos usuários simultaneamente, <b>permitindo que sejam escaláveis</b> conforme as necessidades da aplicação.

### Mundo Fechado e mini-Mundo
"Mundo fechado" geralmente se refere a um <i>sistema ou ambiente</i> em que tem <b>pouca interação ou comunicação</b> com o mundo exterior. No Banco de Dados, <b>se refere</b> a uma representação simplificada de um ambiente do mundo real em um banco de dados.

Um exemplo de "mundo fechado" pode ser uma <i>prisão de segurança máxima</i>, em que os presos têm <b>pouca ou nenhuma</b> interação com o mundo exterior. Já um exemplo de "mini mundo do banco de dados" pode ser um <i>sistema de gerenciamento de biblioteca</i>, em que informações como títulos de livros, autores e empréstimos <b>são armazenadas e gerenciadas</b> em um banco de dados.

### Álgebra Relacional e Projeto de Banco de Dados
A "álgebra relacional do banco de dados" é um <b>conjunto de operações</b> que permitem <b>manipular dados armazenados</b> em um banco de dados relacional. Essas operações incluem <i>seleção, projeção, união, interseção, diferença e junção, entre outras (muito semelhante a matemática)</i>. A <b>álgebra relacional</b> é uma linguagem formal usada para <b>especificar consultas</b> em bancos de dados relacionais.

Já o "projeto de banco de dados" é o processo de <b>projetar a estrutura</b> de um banco de dados, incluindo as <i>tabelas, relacionamentos e restrições</i>. O projeto de banco de dados envolve a <i>identificação dos requisitos de informação e a organização</i> desses requisitos em uma <b>estrutura lógica</b> que possa ser implementada em um sistema de gerenciamento de banco de dados. Um projeto de banco de dados bem feito é <b>fundamental</b> para garantir a <b>integridade e a consistência</b> dos dados armazenados.

### Modelagem
Modelagem é o <b>processo de criação</b> de um modelo abstrato de um sistema ou processo real. A modelagem pode ser usada em diversas áreas, como <i>engenharia, ciência, negócios e computação</i>, e tem como objetivo <b>simplificar a compreensão</b> do sistema ou processo em questão.

Na computação, a modelagem pode ser usada para <i>criar modelos de dados, processos de negócios, interfaces de usuário e sistemas de software</i>. Esses modelos ajudam a <b>visualizar e entender</b> como o sistema ou processo funciona, permitindo a <i>identificação de problemas, a análise de desempenho e a implementação de melhorias</i>.

A modelagem geralmente envolve o <i>uso de diagramas, gráficos ou outras representações visuais</i> para mostrar as relações entre diferentes partes do sistema ou processo. Esses modelos podem ser usados para comunicar <b>ideias e conceitos complexos</b> de forma clara e concisa.

## Modelo de Entidade Relacionamento com Banco de Dados
Em um<b> Modelo de Entidade-Relacionamento (ER)</b>, as entidades representam <b>objetos ou conceitos</b> do mundo real que possuem <b>atributos e relacionamentos</b> com outras entidades. O modelo ER é comumente usado na modelagem de banco de dados para <i>ajudar a organizar e entender a estrutura dos dados</i>.

Em um <b>modelo ER</b>, as <i>entidades são representadas por retângulos e os atributos são representados por elipses conectadas a esses retângulos</i>. Os relacionamentos entre as <i>entidades são representados por linhas conectando as entidades, com um rótulo na linha que descreve a natureza do relacionamento</i>. Além disso, os diagramas ER podem incluir símbolos adicionais para <b>representar restrições e cardinalidade</b> de relacionamentos.

No processo de modelagem de um banco de dados, um diagrama ER <i>pode ajudar a visualizar</i> a estrutura geral dos dados e a <i>identificar problemas ou inconsistências</i> potenciais na estrutura. Com base no diagrama ER, é possível <b>criar um esquema</b> de banco de dados que reflita a estrutura do modelo e forneça uma <i>base para o armazenamento e manipulação de dados</i>.

### Modelo ER: tipos de Entidade, Chaves e Atributos
Um <b>Modelo ER (Entidade-Relacionamento)</b> é uma ferramenta usada para <i>modelar e representar</i> um banco de dados. Existem <b>três componentes principais</b> em um Modelo ER: <i>entidades, chaves e atributos</i>.

<b>Entidades</b> são <i>objetos ou conceitos</i> do mundo real que podem ser <i>identificados e representados</i> no banco de dados. Por exemplo, em um banco de dados de uma empresa, as entidades podem ser <i>clientes, produtos e pedidos</i>.

As <b>chaves</b> são usadas para <i>identificar exclusivamente</i> cada instância de uma entidade. Por exemplo, para uma <i>entidade de cliente</i>, o número do CPF <i>pode ser usado como chave</i>.

<b>Atributos</b> são <i>características das entidades</i> que são armazenadas no banco de dados. Eles <b>descrevem</b> as propriedades de uma entidade. Por exemplo, para uma entidade de produto, os atributos podem ser o nome do <i>produto, preço e descrição</i>.

Ao criar um modelo ER, é <b>importante identificar</b> todas as <i>entidades relevantes</i> e seus <i>atributos</i>, bem como as chaves que serão usadas para identificá-las exclusivamente. Isso ajudará a garantir a integridade dos dados e facilitar a recuperação de informações no banco de dados.

### Relacionamentos, Papéis e Constraints estruturais
<b>Relacionamentos</b> referem-se às <i>conexões ou ligações</i> entre <i>entidades ou elementos de um sistema</i>. Esses relacionamentos podem ser de diferentes tipos, como <i>um-para-um (1:1), um-para-muitos (1:n) ou muitos-para-muitos (n:n)</i>.

<b>Papéis</b> são as <i>funções ou responsabilidades</i> atribuídas a uma entidade em um sistema. Por exemplo, em um sistema de gerenciamento de clientes, um cliente pode desempenhar o papel de <i>comprador ou vendedor</i>.

<b>Constraints estruturais</b> são <i>restrições que limitam</i> as possibilidades de configuração ou operação de um sistema. Essas restrições podem ser físicas, como o tamanho de um objeto ou a capacidade de uma máquina, ou lógicas, como a exigência de que uma determinada operação seja realizada antes de outra.

No contexto do <b>design de sistemas</b>, é importante considerar cuidadosamente os <i>relacionamentos, papéis e constraints estruturais</i> para garantir que o sistema seja <i>funcional, eficiente e seguro</i>.

### Alternativa UML (Unified Modeling Language)
A <b>UML (Unified Modeling Language)</b> é uma linguagem de modelagem padrão que pode ser usada para <i>projetar sistemas, incluindo bancos de dados</i>.

A UML pode ser usada para <i>modelar diferentes aspectos</i> de um banco de dados, como suas <i>entidades, relacionamentos, atributos e restrições</i>. Algumas das principais ferramentas UML que podem ser usadas para modelagem de bancos de dados incluem <i>diagramas de classes, diagramas de entidade-relacionamento (ER), diagramas de sequência e diagramas de atividades</i>.

O <b>diagrama de classe da UML</b> pode ser usado para modelar as classes de <i>objetos do banco de dados, seus atributos e métodos</i>. O diagrama de ER pode ser usado para <i>modelar as entidades e seus relacionamentos</i>, incluindo a <i>cardinalidade e a participação</i>. O <b>diagrama de sequência</b> pode ser usado para modelar como as diferentes entidades interagem e trocam informações, e o diagrama de atividade pode ser usado para modelar o fluxo de trabalho de um processo de banco de dados.

Ao <b>modelar</b> um banco de dados usando a UML, é <b>importante considerar</b> os requisitos do sistema, as restrições de integridade e as boas práticas de design de banco de dados. Uma modelagem bem-feita pode facilitar a criação de um banco de dados <i>eficiente, escalável e de fácil manutenção</i>.

## Modelo de Relacionamento de Entidade Aprimorado com Banco de Dados
O <b>Modelo de Relacionamento de Entidade Aprimorado (ER)</b> é uma <i>técnica para modelagem de dados</i> que permite criar um esquema lógico de um banco de dados. Ele é composto por <i>entidades, atributos e relacionamentos</i>, que <b>representam o que deve ser armazenado</b> no banco de dados.

No <b>modelo ER aprimorado</b>, são utilizados conceitos avançados de modelagem de dados, como <i>generalização/especialização, agregação e entidades fracas</i>. Essas técnicas permitem uma representação mais precisa e completa dos dados, e possibilitam uma <b>melhor estruturação</b> do banco de dados.

No geral, o modelo ER aprimorado é uma <b>forma mais sofisticada</b> de modelar um banco de dados, que leva em consideração a <b>complexidade dos dados</b> que serão armazenados e as <b>necessidades do sistema</b> que os utilizará. Ele é amplamente utilizado em <i>projetos de software e em sistemas de gestão de bancos de dados</i>, sendo uma ferramenta valiosa para garantir a <i>integridade e a eficiência</i> dos dados armazenados.

### Modelo EER
O <b>modelo EER (Entidade-Relacionamento Estendido)</b> é uma <b>variação do modelo ER (Entidade-Relacionamento)</b> utilizado em bancos de dados para <i>representar e descrever as relações</i> entre as entidades. O <b>modelo EER estende o modelo ER</b>, permitindo que os relacionamentos possam ter atributos próprios, além de suportar a definição de subclasses e superclasses, o que possibilita uma melhor organização e representação dos dados. Além disso, o modelo EER também <i>oferece recursos para representar generalização e especialização de entidades</i>, bem como <i>restrições de integridade complexas</i>.

###  Herança
<b>Herança no banco de dados</b> é um <i>conceito utilizado em modelagem de dados que permite</i> a criação de uma nova entidade a partir de uma entidade já existente. Esse processo é conhecido como <i>especialização e generalização de </i>.

Na herança, a <i>entidade original é chamada de superclasse</i>, enquanto a <i>nova entidade criada a partir dela é chamada de subclasse</i>. A <b>subclasse herda</b> todos os atributos e relacionamentos da superclasse e pode ter atributos adicionais próprios.

A herança pode ser implementada em bancos de dados relacionais utilizando <b>duas estratégias principais</b>: <i>tabela única e múltiplas tabelas</i>. Na estratégia de tabela única, os dados de todas as entidades (superclasse e subclasses) são <i>armazenados em uma única tabela</i>, com um campo indicando o <b>tipo</b> da entidade. Já na estratégia de múltiplas tabelas, cada entidade (superclasse e subclasses) é <i>armazenada em uma tabela separada</i>.

A escolha da estratégia depende da <b>complexidade</b> do modelo de dados e das consultas que serão <i>realizadas no banco de dados</i>. A herança no banco de dados é uma <b>técnica poderosa</b> que ajuda a <i>melhorar</i> a organização dos dados e <i>facilitar</i> consultas, mas deve ser utilizada com <b>cuidado</b> para evitar <i>problemas de desempenho e complexidade excessiva</i>.

Exemplos:
Vamos supor que estamos modelando um <b>sistema de gerenciamento</b> de uma biblioteca e queremos utilizar o conceito de <b>herança</b> no banco de dados para representar <i>diferentes tipos de usuários da biblioteca</i>.

Começamos criando uma tabela para a entidade <b>"Usuário"</b>, que será a nossa <b>superclasse</b>. Ela terá os atributos comuns a todos os tipos de usuários:
<code>
	CREATE TABLE Usuario (
  id INT PRIMARY KEY,
  nome VARCHAR(100),
  email VARCHAR(100),
  senha VARCHAR(100)
);
</code>

Agora, vamos criar duas subclasses de usuário: <i>"Aluno"</i> e <i>"Professor"</i>. A classe "Aluno" terá o atributo "curso" e a classe "Professor" terá o atributo "departamento". Para isso, podemos utilizar a estratégia de <b>múltiplas tabelas</b>:
<code>
	CREATE TABLE Aluno (
  id INT PRIMARY KEY,
  nome VARCHAR(100),
  email VARCHAR(100),
  senha VARCHAR(100),
  curso VARCHAR(100)
);

CREATE TABLE Professor (
  id INT PRIMARY KEY,
  nome VARCHAR(100),
  email VARCHAR(100),
  senha VARCHAR(100),
  departamento VARCHAR(100)
);
</code>
Note que as tabelas <i>"Aluno"</i> e <i>"Professor"</i> herdam os atributos da tabela <b>"Usuário"</b>, mas adicionam os seus próprios atributos.

Por fim, podemos criar uma tabela de <b>empréstimo de livros</b>, que relaciona um usuário a um livro emprestado:
<code>
	CREATE TABLE Emprestimo (
  id INT PRIMARY KEY,
  id_usuario INT,
  id_livro INT,
  data_emprestimo DATE,
  data_devolucao DATE,
  FOREIGN KEY (id_usuario) REFERENCES Usuario(id),
  FOREIGN KEY (id_livro) REFERENCES Livro(id)
);
</code>
Ao utilizar o <b>conceito de herança</b> no banco de dados, podemos representar diferentes tipos de <i>usuários (alunos e professores)</i> com atributos específicos, sem precisar duplicar informações na tabela "Usuário". Isso torna a modelagem <b>mais organizada e fácil de entender</b>.

### Especialização e Generalização
<b>Especialização e generalização</b> são conceitos utilizados em modelagem de dados para representar a <i>relação hierárquica entre entidades</i>.

A <b>especialização</b> é o processo de <i>criar uma nova entidade a partir de uma entidade existente</i>, adicionando atributos específicos. Por exemplo, podemos ter a entidade <b>"Pessoa"</b> e criar a entidade <i>"Cliente"</i> a partir dela, adicionando os atributos <i>"data de cadastro"</i> e <i>"limite de crédito"</i>. A entidade <i>"Cliente"</i> é uma especialização da entidade <i>"Pessoa"</i>.

A <i>generalização</i> é o <i>processo contrário</i>, ou seja, é o processo de <i>criar uma nova entidade</i> que abrange outras entidades existentes, combinando seus atributos comuns. Por exemplo, podemos ter as entidades <b>"Cliente"</b> e <b>"Fornecedor"</b> e criar a entidade <i>"Pessoa Jurídica"</i> que abrange ambas, combinando os atributos comuns como <i>"CNPJ"</i> e <i>"razão social"</i>. A entidade <i>"Pessoa Jurídica"</i> é uma generalização das entidades <b>"Cliente"</b> e <b>"Fornecedor"</b>.

A <b>especialização e generalização</b> podem ser representadas em bancos de dados de diversas formas. Uma das formas mais comuns é utilizar a <i>herança de tabelas</i>, como explicado anteriormente. Outra forma é <i>utilizar uma tabela para a entidade geral (superclasse)</i> e outras <i>tabelas para as entidades especializadas (subclasses)</i>, utilizando <b>chaves estrangeiras</b> para relacioná-las.

A escolha da forma de representação depende da <b>complexidade do modelo</b> de dados e das <b>consultas que serão realizadas</b> no banco de dados. A especialização e generalização são <b>técnicas poderosas</b> que ajudam a melhorar a organização dos dados e facilitar consultas, mas devem ser utilizadas com <i>cuidado para evitar problemas de desempenho e complexidade excessiva</i>.

### Hierarquia e Rede de Especialização
<b>Hierarquia e Rede de Especialização</b> são duas formas diferentes de <i>modelar relações entre entidades em um banco de dados</i>.

A <b>Hierarquia</b> é uma forma de representar <i>relações entre entidades em uma estrutura de árvore, onde cada entidade possui um único pai, exceto a raiz da árvore</i>. Por exemplo, em uma <i>hierarquia de funcionários</i> de uma empresa, cada funcionário possui <i>um único gerente</i>, <i>exceto o CEO</i> da empresa que é a <b>raiz da árvore</b>. A hierarquia é uma forma comum de <i>representar estruturas organizacionais ou genealógicas</i>.

Já a <b>Rede de Especialização</b> é uma forma de representar <i>relações entre entidades que podem ter múltiplas especializações</i>. Cada entidade pode ter <i>várias especializações</i>, e cada especialização pode ter <i>outras especializações</i>. Por exemplo, em um banco de dados de <b>animais, pode haver uma entidade <b>"mamífero"</b> que tem especializações como <i>"cão", "gato" e "rato"</i>, e cada uma dessas especializações pode ter suas próprias especializações, como <i>"pastor alemão", "siamese" e "rato de laboratório"</i>. A rede de especialização é uma forma comum de <i>representar classificações taxonômicas ou estruturas de produto</i>.

Ambas as formas de modelagem de dados têm seus <b>usos e limitações</b>, e a <i>escolha entre elas depende do contexto e dos requisitos</i> do banco de dados em questão.

Por exemplo, suponha que você tenha uma tabela <b>"Funcionários"</b> em seu banco de dados e gostaria de definir uma <b>hierarquia de cargos</b> e <b>especializações</b> para cada funcionário.
<b>• Hierarquia:</b> Você pode usar um campo <i>"Cargo"</i> para definir a hierarquia de cargos. Por exemplo, você pode ter cargos como <i>"Presidente", "Diretor", "Gerente" e "Funcionário"</i>. Cada cargo terá uma <i>posição hierárquica diferente</i>. Para tornar isso mais explícito, você pode criar um campo adicional <i>"Nível"</i> que reflete a <b>posição hierárquica</b> de cada cargo. Por exemplo, o <b>"Presidente"</b> pode ter um <b>nível de 1</b>, enquanto um <b>"Funcionário"</b> pode ter um <b>nível de 4</b>.
<br>
<b>• Rede de especialização:</b> Além da <i>hierarquia de cargos</i>, você pode definir uma <i>rede de especialização</i> para cada funcionário. Por exemplo, você pode ter habilidades especializadas como <i>"Programação", "Design", "Gestão de Projetos" e "Vendas"</i>. Cada funcionário pode ter <i>habilidades diferentes</i> e uma classificação para cada habilidade. Por exemplo, um funcionário pode ter uma classificação de <b>3</b> em <b>"Programação"</b> e uma classificação de <b>2</b> em <b>"Design"</b>. Essa classificação pode ser usada para determinar quais funcionários são mais <b>adequados</b> para determinadas tarefas ou projetos.

Essa hierarquia e rede de especialização podem ser representadas em uma única tabela <b>"Funcionários"</b> com campos adicionais para refletir a <i>posição hierárquica e habilidades especializadas</i> de cada funcionário.</b>

### Modelagem de Union types usando Categorias
<b>Union Types</b> em bancos de dados é um <i>conceito relacionado a tipos de dados</i> que podem armazenar <i>mais de um tipo de informação em uma única coluna</i>. Esses tipos são chamados de <i>tipos de união ou tipos compostos</i>, pois eles unem diferentes tipos de dados em um único tipo.

Por exemplo, em um banco de dados que armazena <i>informações de funcionários</i>, a coluna <b>"telefone"</b> pode ser definida como um tipo de união que pode armazenar tanto números de telefone fixo quanto números de celular. Isso permite que uma única coluna acomode <b>diferentes tipos de dados</b> sem a necessidade de criar colunas separadas para cada tipo de telefone.

Os <b>tipos de união (union types)</b> são úteis para lidar com dados variáveis e não estruturados, como <i>listas, conjuntos, dicionários e outras estruturas de dados complexas</i>. Eles também podem ser usados para <i>simplificar</i> a modelagem de dados e <i>reduzir</i> o número de colunas necessárias em um banco de dados.

A ideia por trás dessa técnica é <i>utilizar as Categorias para definir</i> os diferentes tipos de dados que podem ser armazenados em uma coluna, e assim <b>garantir</b> que apenas valores válidos sejam <i>inseridos nessa coluna</i>.

Por exemplo, imagine que temos uma tabela de produtos em um sistema de vendas online, e que alguns produtos podem ter mais de um tipo de cor. <i>Ao invés de criar uma coluna separada para cada tipo de cor</i> (por exemplo, "cor_primaria" e "cor_secundaria"), podemos <i>usar a modelagem de Union types com Categorias</i> para criar uma única coluna "cor" que possa armazenar diferentes tipos de cores.

Para isso, criamos uma <i>tabela de Categorias para armazenar todos os tipos de cores possíveis</i>, como "vermelho", "azul", "verde", etc. Em seguida, associamos essa tabela à coluna "cor" da tabela de produtos, indicando que apenas <i>valores que estejam</i> na tabela de Categorias <i>podem ser inseridos</i> nessa coluna. Dessa forma, <b>podemos garantir</b> que apenas valores válidos de cor sejam inseridos na tabela de produtos, <i>mesmo que alguns produtos tenham mais de uma cor</i>.

A modelagem de Union types usando Categorias é uma <b>técnica poderosa</b> que pode simplificar a modelagem de dados em bancos de dados, reduzindo a necessidade de criar colunas separadas para diferentes tipos de dados. No entanto, é <b>importante lembrar</b> que essa técnica deve ser usada com cuidado e apenas em situações em que os dados são variáveis e não estruturados, pois em outras situações pode ser mais adequado usar colunas separadas para cada tipo de dado.

## Explorando a Linguagem de Consulta a Banco de Dados SQL
## Modelo Relacional e Mapeamento Relacional com Banco de Dados

O <b>Modelo Relacional</b> é um modelo de dados utilizado em bancos de dados que <i>representa as informações em forma de tabelas</i>, onde cada tabela representa uma entidade e cada coluna representa um atributo dessa entidade. As relações entre as tabelas <i>são estabelecidas por meio de chaves estrangeiras</i>, que são utilizadas para relacionar registros em diferentes tabelas.

O <b>Mapeamento Relacional</b> é o processo de <i>converter o modelo de dados de uma aplicação</i> em um modelo que possa ser armazenado em um banco de dados relacional. Esse processo envolve a <i>criação de tabelas e a definição das relações</i> entre elas, de forma a garantir que os dados sejam armazenados de forma <i>eficiente e consistente</i>.

Para realizar o <b>Mapeamento Relacional</b>, é necessário definir as tabelas que serão utilizadas para <i>armazenar os dados da aplicação e as relações entre essas tabelas</i>. Para isso, é importante entender a estrutura da aplicação e como os dados são relacionados entre si.

Por exemplo, imagine que temos uma aplicação de <b>gerenciamento de vendas</b>, onde cada venda é realizada por um vendedor e possui diversos produtos vendidos. Nesse caso, podemos definir três tabelas: <i>uma para os vendedores, uma para os produtos e uma para as vendas</i>. A tabela de vendas teria chaves estrangeiras para as tabelas de vendedores e produtos, estabelecendo as relações entre essas entidades.

<code>
	CREATE TABLE vendas (
    id_venda INT PRIMARY KEY,
    id_vendedor INT,
    id_produto INT,
    quantidade INT,
    valor_total DECIMAL(10,2),
    data_venda DATE,
    FOREIGN KEY (fk_id_vendedor) REFERENCES vendedores (id_vendedor),
    FOREIGN KEY (fk_id_produto) REFERENCES produtos (id_produto)
);
</code>
Sendo -
<b>id_venda:</b> é a chave primária da tabela de vendas, usada para identificar exclusivamente cada venda.
<b>fk_id_vendedor:</b> é a chave estrangeira que se relaciona com a tabela de vendedores, indicando o vendedor responsável pela venda.
<b>fk_id_produto:</b> é a chave estrangeira que se relaciona com a tabela de produtos, indicando o produto vendido.
<b>quantidade:</b> é a quantidade do produto vendido.
<b>valor_total:</b> é o valor total da venda.
<b>data_venda:</b> é a data em que a venda foi realizada.

As cláusulas <b>FOREIGN KEY</b> são usadas para <i>estabelecer as relações</i> entre as tabelas. Elas especificam que as colunas id_vendedor e id_produto são <b>chaves estrangeiras</b> que se <i>relacionam</i> com as tabelas vendedores e produtos.

Além disso, é importante <b>definir os tipos</b> de dados que serão utilizados em cada coluna da tabela, garantindo que os dados sejam armazenados de forma <i>consistente e eficiente</i>. É comum utilizar tipos de dados padrão do banco de dados, como <b>VARCHAR</b> para texto e <b>INT</b> para números inteiros.

O <b>Mapeamento Relacional</b> é uma etapa importante no desenvolvimento de uma aplicação que utiliza banco de dados, pois <i>define como os dados serão armazenados e relacionados entre si</i>. Um bom mapeamento pode <i>garantir a eficiência e consistência dos dados</i>, enquanto um mapeamento inadequado pode levar a <i>problemas de desempenho e inconsistência de dados</i>.

### Comceitos do modelo relacional: Tupla, Atributo e Relação
O <b>modelo relacional</b> é um modelo de dados que organiza as informações em tabelas chamadas de relações. Nesse modelo, existem três conceitos fundamentais: <b>tupla, atributo e relação</b>.

<b>• Tupla:</b> é uma linha específica de uma relação e representa uma <i>entidade ou um conjunto</i> de entidades relacionadas. Por exemplo, em uma tabela de clientes, cada tupla representaria um cliente específico.

<b>• Atributo:</b> é uma <b>coluna específica</b> de uma relação e representa uma <i>característica ou propriedade</i> da entidade representada pela tupla. Por exemplo, em uma tabela de clientes, os atributos poderiam ser o <i>nome, endereço, telefone e e-mail</i>.

<b> • Relação:</b> é uma tabela que contém um <b>conjunto de tuplas e seus atributos</b>. Ela representa um conjunto de entidades que têm <b>características semelhantes</b>. Por exemplo, uma tabela de clientes pode ser uma <i>relação que contém informações</i> sobre todos os clientes de uma empresa.

Esses conceitos são <b>fundamentais</b> para o modelo relacional e são utilizados para <i>representar e manipular</i> dados em bancos de dados relacionais.

## Primeiros Passos com SQL
SQL é uma <b>linguagem de consulta estruturada</b> usada para <i>gerenciar e manipular</i> dados em bancos de dados relacionais. Aqui estão alguns passos para começar com SQL:

<b>• Instale um banco de dados:</b> Você precisa instalar um banco de dados para começar a <b>trabalhar com SQL</b>. Existem muitos bancos de dados disponíveis, como <i>MySQL, Oracle, SQL Server, PostgreSQL, etc.</i> Escolha um banco de dados e instale-o em seu computador.

<b>• Aprenda a sintaxe SQL:</b> A <i>sintaxe SQL</i> é a maneira como você escreve consultas SQL para interagir com o banco de dados. Existem muitos recursos disponíveis on-line para aprender a sintaxe SQL, como <i>tutoriais, cursos e documentação do banco de dados</i>.

<b>• Comece com comandos básicos:</b> Para começar, aprenda alguns comandos básicos do SQL, como <i>SELECT, INSERT, UPDATE e DELETE</i>. Esses comandos permitem <i>selecionar dados, inserir novos dados, atualizar dados existentes e excluir dados do banco de dados</i>.

<b>• Pratique com exemplos:</b> Para aprender SQL, você precisa praticar com exemplos. Use exemplos de bancos de dados ou crie um banco de dados simples para <i>praticar seus comandos SQL</i>.

<b>• Use ferramentas de gerenciamento de banco de dados:</b> Para interagir com o banco de dados, você pode usar ferramentas de gerenciamento de banco de dados, como o <i>MySQL Workbench, o Oracle SQL Developer ou o Microsoft SQL Server Management Studio</i>.

<b>• Aprenda sobre relações:</b> Os bancos de dados relacionais são projetados para armazenar dados em tabelas relacionadas. Aprenda sobre relacionamentos de tabela e como criar consultas que unem várias tabelas. Um bom exemplo é o Modelo Entidade Relacionamento que vimos anteriormente.

<img src="img/yoda-pratice.jpg">

### Sublinguagens: Classificação de SQL - DDL
<b>DDL (Data Definition Language)</b> é uma <i>sublinguagem do SQL (Structured Query Language)</i> que é usada para <i>definir a estrutura e as características</i> dos dados em um banco de dados. Ela é composta por comandos que permitem a <i>criação, alteração e exclusão de objetos do banco de dados</i>, como <i>tabelas, índices, chaves primárias e estrangeiras, entre outros</i>.

Os <b>principais comandos</b> da DDL são:

<b>• CREATE:</b> usado para <b>criar objetos</b> no banco de dados, como <i>tabelas, índices, visões e procedimentos armazenados</i>.
<br>
<b>• ALTER:</b> usado para <b>alterar a estrutura</b> dos objetos do banco de dados, como <i>adicionar ou remover</i> colunas de uma tabela.
<br>
<b>• DROP:</b> usado para <b>excluir objetos</b> do banco de dados, como <i>tabelas, visões e índices</i>.
<br>
<b>• TRUNCATE:</b> usado para <b>excluir todos os dados</b> de uma tabela sem excluir a própria tabela.
<br>
<b>• RENAME:</b> usado para <b>renomear objetos</b> do banco de dados, como tabelas e colunas.

Esses comandos da DDL são <b>muito importantes</b> para o gerenciamento de um banco de dados, pois permitem a <i>criação, alteração e exclusão</i> de objetos do banco de dados de forma <i>eficiente e organizada</i>. Além disso, eles garantem que os dados armazenados estejam estruturados de acordo com as necessidades do usuário e da aplicação que utiliza o banco de dados.

Segue um exemplo:
Suponha que você queira criar uma tabela chamada <b>"Clientes"</b> para armazenar informações sobre os clientes de uma loja. Você pode usar o seguinte código DDL do SQL para criar a tabela:
<code>
	CREATE TABLE Clientes (
   id INT PRIMARY KEY,
   nome VARCHAR(50),
   email VARCHAR(50),
   telefone VARCHAR(15),
   endereco VARCHAR(100)
);
</code>
Este código cria uma tabela chamada "Clientes" com cinco colunas: "id", "nome", "email", "telefone" e "endereco". A coluna "id" é definida como a chave primária da tabela usando o comando "PRIMARY KEY". As outras colunas são definidas como campos de texto usando o tipo "VARCHAR" e o tamanho máximo de cada campo é especificado entre parênteses.

Suponha que você precise <b>adicionar uma nova coluna</b> chamada <b>"idade"</b> à tabela <b>"Clientes"</b> que criamos anteriormente. Você pode usar o seguinte código DDL do SQL para adicionar a nova coluna:
<code>
	ALTER TABLE Clientes
ADD idade INT;
</code>
Este código usa o comando <b>"ALTER TABLE"</b> para <i>modificar a tabela</i> <b>"Clientes"</b> e <b>adiciona uma nova</b> coluna chamada <b>"idade"</b> do tipo <b>inteiro (INT)</b>. Depois de executar este código, a tabela <b>"Clientes"</b> terá uma nova coluna chamada <b>"idade"</b>.

Agora, se você quiser adicionar dados à nova coluna <b>"idade"</b> da tabela <b>"Clientes"</b>, pode usar o seguinte código SQL:
<code>
	UPDATE Clientes
SET idade = 30
WHERE id = 1;
</code>
Este código SQL usa o comando <b>"UPDATE"</b> para <b>alterar os dados</b> da tabela <b>"Clientes"</b>. O comando <b>"SET" define o valor</b> da coluna <b>"idade"</b> como 30. O comando <b>"WHERE" especifica</b> que apenas a linha com o valor de "id" igual a 1 <i>deve ser atualizada</i>. Após a execução deste código, a linha com o "id" 1 na tabela <b>"Clientes"</b> terá o valor <b>"idade"</b> definido como 30.

Suponha que você não precise mais da tabela <b>"Clientes"</b> que criamos anteriormente e deseja <b>excluí-la</b> do seu banco de dados. Você pode usar o seguinte código DDL do SQL para <i>excluir a tabela</i>:
<code>
	DROP TABLE Clientes;
</code>
Este código usa o comando <b>"DROP TABLE"</b> para <b>excluir completamente</b> a tabela "Clientes" do seu banco de dados. Depois de executar este código, a tabela "Clientes" e todos os seus dados serão <b>permanentemente excluídos</b>.

É <b>importante</b> notar que o comando <b>"DROP TABLE"</b> é <b>IRREVERSÍVEL</b> e <i>deve ser usado com cuidado</i>. Se você excluir uma tabela acidentalmente, <i>perderá todos os dados armazenados</i> nela e <b>não poderá recuperá-los</b>. Portanto, é recomendável sempre fazer um backup de seus dados antes de executar comandos DDL que possam afetar suas tabelas.

## Explorando Queries com SQL
Explorar queries com SQL é uma <b>habilidade essencial</b> para trabalhar com bancos de dados. Aqui estão algumas etapas para começar:

<b>• Entenda sua estrutura de dados:</b> Antes de começar a escrever consultas, é importante que você <i>entenda a estrutura</i> do banco de dados, incluindo as <i>tabelas, colunas e relacionamentos</i>.

<b>• Escreva consultas simples:</b> Comece escrevendo consultas simples para <b>selecionar dados</b> de uma tabela específica. Use a cláusula <b>SELECT</b> para <b>selecionar as colunas</b> que você precisa e a cláusula <b>FROM</b> para <b>especificar a tabela</b>.

<b>• Use a cláusula WHERE para filtrar resultados:</b> Para <i>refinar seus resultados</i>, use a cláusula <b>WHERE</b> para filtrar com <i>base em condições específicas.</i>

<b>• Combine múltiplas tabelas com JOIN:</b> Se você <b>precisar combinar</b> dados de várias tabelas, use a cláusula <b>JOIN</b> para <b>unir</b> as tabelas.

<b>• Agrupe e resuma dados com GROUP BY e funções agregadas:</b> Se você precisar <b>agrupar dados</b> por uma ou mais colunas e <b>realizar cálculos</b> resumidos, como <i>somas ou contagens</i>, use a cláusula <b>GROUP BY</b> e funções agregadas como <b>SUM e COUNT</b>.

<b>• Ordene resultados com ORDER BY:</b> Para <b>ordenar</b> seus resultados por <i>uma ou mais</i> colunas, use a cláusula <b>ORDER BY</b>.

<b>• Use subconsultas para consultas complexas:</b> Se você precisar de consultas mais complexas, use <b>subconsultas</b> para criar consultas dentro de consultas.

<b>Experimente e refine suas consultas:</b> Experimente diferentes consultas para ver <b>quais retornam</b> os resultados desejados e <b>refine suas consultas</b> para torná-las mais eficientes.

Com <b>prática e experiência</b>, você pode se tornar um expert em escrever consultas SQL e <b>obter insights</b> valiosos de seus dados.

### Comandos Baseados em Operações Matemáticas: UNION, INTERSECTION e EXCEPT
Esses comandos são usados para <b>combinar resultados</b> de consultas diferentes ou para <b>obter um conjunto</b> de resultados que satisfazem uma condição específica.

<b>• UNION:</b>
O comando UNION é usado para <b>combinar os resultados</b> de duas ou mais consultas <b>SELECT</b> em um único conjunto de resultados. Ele remove quaisquer duplicatas do conjunto de resultados final. A <b>sintaxe</b> do comando UNION é a seguinte:
<code>
	SELECT coluna1, coluna2 FROM tabela1
UNION
SELECT coluna1, coluna2 FROM tabela2;
</code>
Aqui, duas consultas SELECT são combinadas usando o comando UNION.
<b>• INTERSECT:</b>
O comando <b>INTERSECT</b> é usado para <b>retornar os resultados</b> comuns de duas ou mais consultas <b>SELECT</b>. Ele retorna apenas as linhas que aparecem em todos os conjuntos de resultados. A <b>sintaxe</b> do comando INTERSECT é a seguinte:
<code>
	SELECT coluna1, coluna2 FROM tabela1
INTERSECT
SELECT coluna1, coluna2 FROM tabela2;
</code>
Aqui, duas consultas <b>SELECT</b> são combinadas usando o comando <b>INTERSECT</b>.
<b>• EXCEPT:</b>
O comando <b>EXCEPT</b> é usado para <b>retornar as linhas</b> que aparecem na <b>primeira consulta</b> SELECT, mas <b>não na segunda</b> consulta SELECT. Ele <i>retorna todas as linhas</i> da primeira consulta SELECT que não aparecem na segunda consulta SELECT. A <b>sintaxe</b> do comando EXCEPT é a seguinte:
<code>
	SELECT coluna1, coluna2 FROM tabela1
EXCEPT
SELECT coluna1, coluna2 FROM tabela2;
</code>
Aqui, duas consultas <b>SELECT</b> são combinadas usando o comando <b>EXCEPT</b>.

Continuando...
<br>
<b>• MOD (%):</b>
O operador <b>MOD</b> é usado para <b>retornar o resto</b> de uma divisão. Por exemplo, se você quiser <i>encontrar todos os registros</i> em uma tabela cujo id seja ímpar, você pode usar o operador MOD da seguinte forma:
<code>
	SELECT * FROM tabela WHERE id % 2 = 1;
</code>
Este comando retornará todos os registros em que o valor da coluna "id" é ímpar.

<b>• EXISTS:</b>
O operador <b>EXISTS</b> é usado para <b>verificar se uma subconsulta</b> retorna algum resultado. Por exemplo, se você quiser verificar se há algum registro na tabela <b>"pedidos"</b> para um determinado cliente, você pode usar o operador <b>EXISTS</b> da seguinte forma:
<code>
	SELECT * FROM clientes WHERE EXISTS(SELECT * FROM pedidos WHERE clientes.id = pedidos.id_cliente);
</code>
Este comando <b>retornará todos</b> os clientes que têm <i>pelo menos um</i> registro na tabela <b>"pedidos"</b>.

Esses comandos podem ser muito <b>úteis para realizar</b> operações mais avançadas em seu banco de dados e <b>obter resultados</b> mais <i>precisos e específicos</i>.

### Elaborando Queries SQL com Expressões
• Consulta que <b>retorna o número</b> de vendas feitas por cada vendedor em <b>ordem decrescente</b>:
<code>
	SELECT vendedor, COUNT(*) as num_vendas 
	FROM tabela_vendas 
	GROUP BY vendedor 
	ORDER BY num_vendas DESC;
</code>
• Consulta que <b>retorna os produtos</b> que tiveram uma quantidade de vendas <b>superior a 1000</b> unidades:
<code>
	SELECT produto 
	FROM tabela_vendas 
	WHERE quantidade_vendida > 1000;
</code>
• Consulta que retorna a média de preço dos produtos vendidos:
<code>
	SELECT AVG(preco) as media_precos 
	FROM tabela_vendas;
</code>
• Consulta que retorna os vendedores que realizaram vendas acima da média:
<code>
	SELECT vendedor 
	FROM tabela_vendas 
	GROUP BY vendedor 
	HAVING AVG(valor_venda) > (SELECT AVG(valor_venda) FROM tabela_vendas);
</code>
• Consulta que retorna o número de vendas realizadas em cada mês do ano atual:
<code>
	SELECT MONTH(data_venda) as mes, COUNT(*) as num_vendas 
	FROM tabela_vendas 
	WHERE YEAR(data_venda) = YEAR(CURRENT_DATE()) 
	GROUP BY mes;
</code>

## Criando Queries com Funções e Cláusulas de Agrupamentos
As funções permitem <b>realizar cálculos e operações</b> em colunas de dados, enquanto as cláusulas de agrupamento permitem <i>agrupar os resultados de uma query</i> com base em <i>uma ou mais</i> colunas específicas.

Algumas <i>funções comuns</i> em SQL incluem:
<b>• SUM():</b> soma os valores de uma coluna
<b>• AVG():</b> calcula a média dos valores de uma coluna
<b>• COUNT():</b> conta o número de registros em uma coluna
<b>• MAX():</b> retorna o valor máximo de uma coluna
<b>• MIN():</b> retorna o valor mínimo de uma coluna

Por exemplo, para <b>obter a soma</b> dos salários de todos os funcionários de uma empresa, poderíamos usar a função <b>SUM()</b> da seguinte forma:
<code>
	SELECT SUM(salario) FROM funcionarios;
</code>
Já as cláusulas de agrupamento, como <b>GROUP BY</b>, são usadas para agrupar os <b>resultados da query</b> com base em uma ou mais colunas. Por exemplo, para <i>obter a soma</i> dos salários de cada departamento da empresa, poderíamos usar a cláusula <b>GROUP BY</b> da seguinte forma:
<code>
	SELECT departamento, SUM(salario) FROM funcionarios GROUP BY departamento;
</code>
Isso <i>retornaria uma tabela</i> com o nome de cada departamento e a <i>soma dos salários</i> de todos os funcionários desse departamento.

### ORDER BY: Cláusulas de ordenação com SQL
O <b>"ORDER BY"</b> é uma <i>cláusula do SQL</i> que é usada para classificar os resultados de uma consulta em uma <i>ordem específica</i>. Essa cláusula é usada em conjunto com a cláusula <b>"SELECT"</b> para <i>especificar as colunas</i> que devem ser <i>retornadas e a ordem</i> em que elas devem ser classificadas.

A <b>sintaxe básica</b> do "ORDER BY" é a seguinte:
<code>
	SELECT coluna1, coluna2, coluna3
	FROM tabela
	ORDER BY coluna1 DESC, coluna2 ASC;
</code>

Neste exemplo, estamos selecionando as colunas <b>"coluna1", "coluna2" e "coluna3"</b> da tabela especificada, e <b>ordenando os resultados</b> pela coluna1 em <b>ordem descendente (DESC)</b> e pela coluna2 em ordem <b>ascendente (ASC)</b>.

Podemos <i>ordenar os resultados</i> de uma consulta usando uma ou mais colunas e especificar a ordem de classificação como <b>ascendente</b> ou <b>descendente</b>. Quando várias colunas são usadas para classificação, a ordem das colunas na cláusula <b>"ORDER BY"</b> determina a prioridade da classificação.

É importante lembrar que a cláusula <b>"ORDER BY"</b> é usada apenas para <i>classificar os resultados de uma consulta</i> e <i>não afeta a estrutura ou o conteúdo da tabela subjacente</i>.

### GROUP BY: Cláusulas de ordenação com SQL
O <b>"GROUP BY"</b> é uma cláusula do SQL que permite <b>agrupar os resultados</b> de uma consulta com base no valor de <i>uma ou mais</i> colunas. Essa cláusula é frequentemente usada em conjunto com funções de agregação, como <i>"SUM", "AVG", "COUNT" e "MAX"</i>, para resumir dados em grupos específicos.

A <b>sintaxe básica</b> do "GROUP BY" é a seguinte:
<code>
SELECT coluna1, coluna2, funcao_agregada(coluna3)
FROM tabela
GROUP BY coluna1, coluna2;
</code>

Neste exemplo, estamos selecionando as colunas <b>"coluna1" e "coluna2"</b> da tabela especificada, e aplicando uma <b>função de agregação (por exemplo, "SUM")</b> à coluna3, <b>agrupando os resultados</b> por "coluna1" e "coluna2".

Ao usar a cláusula <b>"GROUP BY"</b>, devemos especificar todas as colunas que <i>não estão envolvidas</i> em funções de agregação na cláusula <b>"SELECT"</b>. Caso contrário, o SQL <i>gerará um erro</i>.

A cláusula <b>"GROUP BY"</b> é uma <b>ferramenta poderosa</b> para resumir dados em grupos específicos. Com ela, podemos <b>obter informações</b> úteis sobre subconjuntos de dados e <b>tomar decisões</b> de negócios mais informadas. No entanto, é importante usá-la com <b>cuidado</b> e <b>entender</b> como ela <i>afeta os resultados da consulta</i>.

Também é possível usar a cláusula <b>"HAVING"</b> em conjunto com a cláusula <b>"GROUP BY"</b> para <b>especificar uma condição</b> que deve ser satisfeita pelos grupos resultantes. A cláusula <b>"HAVING"</b> é <i>semelhante</i> à cláusula <b>"WHERE"</b>, mas é aplicada aos resultados agrupados em vez dos dados brutos.

A <b>sintaxe básica</b> do "HAVING" é a seguinte:
<code>
SELECT coluna1, funcao_agregada(coluna2)
FROM tabela
GROUP BY coluna1
HAVING funcao_agregada(coluna2) > valor;
</code>

Neste exemplo, estamos selecionando a <b>"coluna1"</b> da tabela especificada e aplicando uma <b>função de agregação (por exemplo, "SUM")</b> à "coluna2", <b>agrupando</b> os resultados por "coluna1". Em seguida, estamos <b>filtrando os resultados</b> usando a cláusula <b>"HAVING"</b> para incluir apenas os grupos com uma soma de "coluna2" <b>maior que</b> um determinado valor.

A cláusula <b>"GROUP BY"</b> pode ser usada para <b>resumir dados</b> em grupos específicos e ajudar a <b>tomar decisões</b> de negócios mais informadas. No entanto, é importante <i>usá-la com cuidado e entender</i> como ela afeta os resultados da consulta.

### Having Statment
A declaração <b>"HAVING"</b> é usada em consultas SQL para <b>filtrar grupos</b> de resultados após o uso da cláusula <b>"GROUP BY"</b>. A cláusula <b>"HAVING"</b> é usada para <i>especificar uma condição que deve ser atendida</i> pelos grupos resultantes.

A principal diferença entre a cláusula <b>"WHERE"</b> e a cláusula <b>"HAVING"</b> é que a primeira é usada para <i>filtrar linhas individuais</i>, enquanto a última é usada para <i>filtrar grupos de resultados</i>. Além disso, a cláusula "HAVING" é <b>sempre usada após</b> a cláusula "GROUP BY".

A <b>sintaxe básica</b> da cláusula "HAVING" é a seguinte:
<code>
SELECT coluna1, coluna2, ...
FROM tabela
GROUP BY coluna1, coluna2, ...
HAVING condição;
</code>

A condição especificada na cláusula "HAVING" pode <i>incluir funções de agregação, como SUM, COUNT, AVG, MAX, MIN, entre outras</i>. Além disso, a condição pode incluir <i>operadores lógicos, como AND, OR e NOT</i>.

Em resumo, a cláusula "HAVING" é uma <b>ferramenta útil</b> para filtrar grupos de resultados em consultas SQL e <i>deve ser usada após a cláusula</i> "GROUP BY".

## Agrupamendo Registros e Tabelas com Join Statment
O Agrupamento de Registros e Tabelas com o Join Statement é uma técnica utilizada em bancos de dados relacionais para <b>combinar dados</b> de duas ou mais tabelas <b>em uma única consulta</b>.

O <b>Join Statement</b> permite que o usuário especifique como as tabelas estão relacionadas entre si, com base em uma ou mais colunas comuns. Essa relação é usada para <b>combinar</b> as linhas das tabelas que possuem valores correspondentes nessas colunas.

Além disso, o <b>Join Statement</b> também permite <b>agrupar os registros</b> resultantes da combinação de tabelas em um único conjunto, com <i>base em uma ou mais colunas selecionadas</i>. Isso é feito por meio do uso da cláusula <b>"GROUP BY"</b>, que especifica <i>quais colunas devem ser usadas para agrupar os resultados</i>.

Existem <b>diferentes tipos de joins</b>, cada um com um <b>comportamento específico</b>. Os mais comuns são:

<b>• Inner Join:</b> retorna apenas as linhas das tabelas que possuem valores correspondentes nas colunas especificadas;
<br>
<b>• Left Join:</b> retorna todas as linhas da tabela da esquerda e as linhas correspondentes da tabela da direita (ou NULL, se não houver correspondência);
<br>
<b>• Right Join:</b> retorna todas as linhas da tabela da direita e as linhas correspondentes da tabela da esquerda (ou NULL, se não houver correspondência);
<br>
<b>• Full Outer Join:</b> retorna todas as linhas de ambas as tabelas, incluindo aquelas que não têm correspondência em nenhuma das tabelas.

O <b>agrupamento de registros e tabelas</b> com o Join Statement é uma técnica <b>poderosa e versátil</b> que permite que os usuários obtenham informações mais completas e precisas de seus bancos de dados. No entanto, é importante lembrar que um <i>uso inadequado do Join Statement pode afetar negativamente o desempenho do banco de dados e resultar em consultas lentas ou falhas</i>. Por isso, é <i>recomendável ter conhecimento e prática</i> em SQL antes de usá-lo em um ambiente de produção.

### CASE Statment
O CASE statement em SQL é uma <b>cláusula condicional</b> que permite <i>avaliar uma expressão e retornar um resultado baseado em uma ou mais condições</i>. Ele pode ser usado em <b>SELECT, WHERE, HAVING e ORDER BY</b> cláusulas para realizar uma <b>lógica condicional</b>.

A <b>sintaxe básica</b> do CASE statement é a seguinte:
<code>
CASE
WHEN condição1 THEN resultado1
WHEN condição2 THEN resultado2
ELSE resultado_padrao
END
</code>

Onde "condição1" e "condição2" são as <b>condições que serão avaliadas</b>, "resultado1" e "resultado2" são os <b>resultados a serem retornados</b> se a condição correspondente <b>for verdadeira</b> e "resultado_padrao" é o <b>resultado a ser retornado se nenhuma</b> das condições anteriores <b>for verdadeira</b>.

Por exemplo, imagine que temos uma tabela de produtos com as colunas <b>"nome", "preço" e "desconto"</b>. Podemos usar um <b>CASE statement</b> <i>para retornar</i> o preço final de cada produto, levando em conta o desconto:
<code>
SELECT nome, preço,
CASE
WHEN desconto > 0 THEN preço * (1 - desconto)
ELSE preço
END AS preço_final
FROM produtos
</code>

Neste caso, estamos avaliando <b>se o desconto é maior que zero</b>. Se for, calculamos o preço final do produto com desconto. Caso contrário, retornamos o preço original.

O CASE statement é uma <b>ferramenta muito útil</b> para trabalhar com <b>lógica condicional</b> em SQL e pode ser usado de diversas maneiras para <i>realizar tarefas complexas</i>.

O CASE statement <b>também pode ser aninhado</b>, permitindo que condições mais complexas sejam avaliadas. Por exemplo, podemos usar um CASE statement <b>dentro de outro</b> CASE statement para <b>avaliar várias</b> condições e retornar um <i>resultado baseado</i> nelas.

A <b>sintaxe</b> do CASE statement aninhado é a seguinte:
<code>
CASE
WHEN condição1 THEN
CASE
WHEN condição2 THEN resultado2
ELSE resultado3
END
ELSE resultado1
END
</code>

Neste exemplo, estamos avaliando <b>duas condições</b>. Se a primeira condição for verdadeira, avaliamos a segunda condição usando outro CASE statement. Se a segunda condição for verdadeira, retornamos o resultado2, caso contrário, retornamos o resultado3. Se a primeira condição for falsa, retornamos o resultado1.

O CASE statement <i>também pode ser usado</i> com funções agregadas, como <i>SUM, COUNT e AVG</i>, para realizar cálculos condicionais em grupos de dados. Isso pode ser muito útil em <i>relatórios e análises de dados complexos</i>.

Em resumo, o CASE statement é uma <b>cláusula condicional muito poderosa</b> em SQL, permitindo que expressões complexas sejam avaliadas e resultados condicionais sejam retornados. Ele é uma <b>ferramenta fundamental</b> em qualquer programação de banco de dados e pode ser usado de várias maneiras para <i>manipular dados de forma eficaz e eficiente</i>.

## O Caso Zero/Null Trick
O caso zero/null trick em SQL é uma técnica usada para <b>retornar valores diferentes</b> de zero em uma consulta SQL.

Em muitos casos, as consultas SQL retornam zero <i>quando não há nenhum registro correspondente nas tabelas consultadas</i>. No entanto, em alguns casos, é necessário retornar um valor diferente de zero, como quando se deseja exibir <i>um valor padrão ou um valor calculado</i>.

Para resolver isso, a técnica zero/null trick <b>envolve o uso</b> de uma subconsulta que retorna um valor nulo quando não há registros correspondentes e, em seguida, utiliza a função <b>COALESCE</b> para retornar o valor desejado.

Por exemplo, se quisermos retornar o número total de vendas de um determinado produto, mas exibir <b>"N/A"</b> em vez de zero quando não houver vendas, poderíamos usar a seguinte consulta:
<code>
	SELECT COALESCE((SELECT SUM(sales) FROM products WHERE product_id = 123), 'N/A') AS total_sales;
</code>

Nesse caso, a subconsulta retorna nulo <b>se não houver nenhum</b> registro correspondente na tabela de produtos, e a função <b>COALESCE</b> substitui esse valor nulo pelo valor <b>"N/A"</b>. <i>Se houver registros correspondentes</i>, a soma das vendas será exibida normalmente.

## Personalizando Acessos com Views
<b>Views são consultas</b> SQL armazenadas que <i>permitem personalizar o acesso aos dados em um banco de dados</i>. Elas podem ser usadas para <b>restringir o acesso</b> a determinadas colunas ou linhas de dados, <b>limitar a exposição</b> de informações sensíveis ou <b>simplificar consultas</b> complexas.

Ao criar uma view, você está criando uma <b>"tabela virtual"</b> que contém os <i>resultados de uma consulta</i>. Você pode definir restrições de acesso para que <b>apenas determinados</b> usuários possam <i>visualizar a view ou apenas permitir</i> que determinados usuários possam executar certas operações na view, como selecionar ou atualizar dados.

Além disso, views também podem ser usadas para <b>simplificar o acesso</b> a dados complexos. Por exemplo, você pode criar uma view que <i>combine várias tabelas</i> em uma única tabela virtual, <b>facilitando</b> a consulta de informações de várias fontes de dados.

Views são uma <b>ferramenta poderosa</b> para personalizar o acesso aos dados em um banco de dados, tornando-o <i>mais seguro, mais simples e mais eficiente</i>.

### Personalizando Acessos com Views no MySQL
Para personalizar um acesso com view no MySQL, pode fazer da seguinte maneira:

<b>• Criar a view:</b> Utilize o comando <b>"CREATE VIEW"</b> para <i>criar a view com os campos</i> que deseja visualizar.
Exemplo:
<code>
CREATE VIEW minha_view AS SELECT coluna1, coluna2 FROM minha_tabela;
</code>

<b>• Conceder acesso à view:</b> Utilize o comando <b>"GRANT SELECT"</b> para <i>conceder acesso à view para um usuário específico</i>.
Exemplo:
<code>
GRANT SELECT ON minha_view TO meu_usuario;
</code>

<b>• Revogar acesso à view:</b> Utilize o comando <b>"REVOKE SELECT"</b> para <b>revogar o acesso</b> à view para um usuário específico.
Exemplo:
<code>
REVOKE SELECT ON minha_view FROM meu_usuario;
</code>

Com esses passos, você pode <b>personalizar o acesso</b> à view no MySQL de acordo com as necessidades do seu projeto.

### Explorando exemplos de criação de views
Uma view é uma <b>tabela virtual</b> que é criada a partir de uma <i>consulta SQL e que pode ser usada como uma tabela real</i>. Ela pode ser usada para <b>simplificar consultas</b> complexas ou para fornecer uma visão mais restrita dos dados para determinados usuários.

Para <b>criar uma view</b>, é necessário usar a <b>sintaxe SQL CREATE VIEW</b>. Aqui está um exemplo:
<code>
CREATE VIEW clientes_ativos AS
SELECT *
FROM clientes
WHERE status = 'ativo';
</code>

Neste exemplo, criamos uma view chamada <b>"clientes_ativos"</b> que contém todos os clientes que têm status <b>"ativo"</b>.

Uma vez criada a view, podemos <b>usá-la em consultas</b> como se fosse uma tabela real. Por exemplo:
<code>
SELECT *
FROM pedidos
INNER JOIN clientes_ativos ON pedidos.cliente_id = clientes_ativos.id;
</code>

Neste exemplo, estamos selecionando todos os pedidos que foram feitos por clientes ativos, usando a view <b>"clientes_ativos"</b> para restringir a lista de clientes.

Outro exemplo de uso de views é para simplificar consultas complexas. 
Segue um exemplo:
<code>
CREATE VIEW vendas_por_mes AS
SELECT
  YEAR(data) AS ano,
  MONTH(data) AS mes,
  SUM(total) AS total_vendido
FROM pedidos
GROUP BY YEAR(data), MONTH(data);
</code>

Neste exemplo, criamos uma view chamada <b>"vendas_por_mes"</b> que calcula o <i>total vendido por mês em cada ano</i>. Isso pode ser útil para análises de vendas ou para gerar gráficos.

As views podem ser úteis para <i>simplificar consultas complexas, fornecer uma visão mais restrita dos dados para determinados usuários e até mesmo para gerar relatórios e gráficos</i>.

## Explorando Cláusulas de DDL e Esquemas de Banco de Dados no MySQL
Como dito anteriormente, <b>DDL</b> significa <b>"Data Definition Language"</b> e é usado para <i>criar, alterar e excluir objetos</i> de banco de dados, como <i>tabelas, índices e visões</i>. Aqui estão algumas das <i>cláusulas DDL mais comuns</i> no MySQL:

<b>• CREATE:</b> <i>cria um novo</i> objeto de banco de dados, como uma tabela, índice ou visão.
<b>• ALTER:</b> <i>modifica a estrutura</i> de um objeto de banco de dados existente, como <i>adicionar ou excluir uma coluna</i> em uma tabela.
<b>• DROP:</b> <i>exclui um objeto</i> de banco de dados existente, como uma tabela ou índice.

Os esquemas de banco de dados no MySQL são uma <b>coleção lógica</b> de objetos de banco de dados, como tables e views. Eles são usados para <i>organizar e gerenciar</i> objetos de banco de dados relacionados. Um esquema é criado usando a cláusula DDL <b>"CREATE SCHEMA"</b>(SCHEMA e DATABASE são os mesmos). Por exemplo:
<code>
CREATE SCHEMA meu_banco_de_dados;
</code>

Uma vez criado o esquema, podemos criar tabelas e outros objetos de banco de dados dentro dele. Aqui está um exemplo de criação de uma tabela dentro do esquema "meu_banco_de_dados":
<code>
CREATE TABLE meu_banco_de_dados.clientes (
  id INT NOT NULL AUTO_INCREMENT,
  nome VARCHAR(50) NOT NULL,
  email VARCHAR(50) NOT NULL,
  PRIMARY KEY (id)
);
</code>

Neste exemplo, criamos uma tabela chamada <b>"clientes"</b> dentro do schema <b>"meu_banco_de_dados"</b>. A tabela contém três colunas: <b>"id", "nome" e "email"</b>. A cláusula <b>"PRIMARY KEY"</b> define a coluna <b>"id"</b> como <b>chave primária</b> da tabela.

Podemos usar a cláusula <b>"USE"</b> para selecionar o schema que queremos usar em uma consulta:
<code>
USE meu_banco_de_dados;
</code>

Isso irá <i>selecionar o esquema</i> <b>"meu_banco_de_dados"</b> para uso em <i>consultas subsequentes</i>.

As cláusulas DDL e os esquemas de banco de dados <b>são importantes</b> para <b>criar e gerenciar</b> objetos de banco de dados no MySQL. Eles nos permitem <b>organizar e controlar</b> melhor os dados em nossos <b>aplicativos e sistemas</b>.

## Lógica de Programação com SQL Dinâmico
A <b>lógica de programação</b> é um <i>conjunto de técnicas utilizadas para desenvolver algoritmos</i> que <b>resolvem problemas</b> computacionais. O <b>SQL dinâmico</b> é uma técnica utilizada para <b>construir instruções</b> SQL em tempo de execução, de acordo com as necessidades do programa.

Para <b>utilizar</b> o SQL dinâmico, é <i>necessário ter um bom entendimento da sintaxe</i> do SQL, bem como da estrutura de banco de dados utilizado. É importante também ter <b>conhecimento sobre</b> os tipos de dados e as operações que podem ser realizadas no SQL.

A <b>lógica de programação</b> pode ser aplicada ao SQL dinâmico para criar instruções SQL mais <i>eficientes e otimizadas</i> para cada situação. Isso envolve a <b>utilização de técnicas</b> de controle de fluxo, como <i>estruturas de decisão e repetição</i>, para criar instruções SQL que <b>atendam às necessidades</b> específicas do programa.

Alguns exemplos de aplicação da <b>lógica de programação</b> com SQL dinâmico incluem a <i>criação de consultas</i> SQL personalizadas com <i>base em dados fornecidos</i> pelo usuário, <i>a geração de relatórios dinâmicos</i> a partir de consultas SQL complexas e a <i>construção de scripts</i> de migração de dados para mover dados de um banco de dados para outro.

A <b>lógica de programação é fundamental</b> para a utilização eficiente do SQL dinâmico, permitindo que os desenvolvedores <i>criem instruções SQL personalizadas e otimizadas</i> para atender às necessidades específicas do programa.

Além disso, é importante <b>mencionar que</b> a lógica de programação com SQL dinâmico pode ser aplicada em diversos tipos de banco de dados, como <i>MySQL, PostgreSQL, SQL Server, Oracle, entre outros</i>.

Outra técnica <b>importante</b> que pode ser <i>utilizada em conjunto com a lógica de programação e o SQL dinâmico</i> é a <b>normalização</b> de banco de dados. A normalização é um processo que <b>permite organizar</b> as informações de um banco de dados de maneira <i>mais eficiente, reduzindo</i> a redundância de dados e <i>garantindo a integridade</i> das informações.

Ao utilizar a <b>normalização de banco de dados</b> em conjunto com a lógica de programação e o SQL dinâmico, é possível criar instruções SQL mais <b>complexas e eficientes</b>, que lidam com tabelas normalizadas e relacionamentos entre elas.

Por fim, é importante mencionar que a lógica de programação com SQL dinâmico é uma <b>habilidade importante</b> para os profissionais de programação e desenvolvimento de banco de dados. Com ela, é possível <i>criar aplicações mais flexíveis, otimizadas e seguras</i>, que atendem às necessidades específicas dos usuários.

Em resumo, a lógica de programação com SQL dinâmico é uma <b>técnica importante</b> que permite a criação de instruções SQL personalizadas e otimizadas, que <b>atendem às necessidades</b> específicas do programa. É importante aplicar <b>boas práticas de segurança</b> ao utilizar o SQL dinâmico, e a normalização de banco de dados<i> pode ser utilizada em conjunto</i> para criar instruções SQL mais complexas e eficientes.

Um <b>exemplo de aplicação</b> da lógica de programação com SQL dinâmico é a criação de uma <i>consulta personalizada para buscar informações</i> em um banco de dados. Suponha que temos uma tabela chamada <b>"Clientes"</b> com as seguintes colunas: <i>ID, Nome, Sobrenome, Email e Telefone</i>.

Em um programa, podemos criar uma tela de busca que permita ao usuário <b>pesquisar clientes</b> com base em diferentes critérios, como <i>nome, sobrenome ou email</i>. Para isso, podemos utilizar o SQL dinâmico para construir a consulta SQL de acordo com o critério selecionado pelo usuário.

Por exemplo, se o usuário deseja <b>buscar clientes</b> pelo nome, podemos construir a consulta SQL dinamicamente da seguinte maneira:
<code>
	DECLARE @nome VARCHAR(50) = 'João';
	DECLARE @sql VARCHAR(MAX);

	SET @sql = 'SELECT * FROM Clientes WHERE Nome = ''' + @nome + '''';

	EXEC (@sql);
</code>
Neste exemplo, a variável <b>@nome</b> contém o valor do nome <b>digitado pelo usuário</b>. A consulta SQL é construída dinamicamente utilizando a função <b>EXEC()</b>, que permite <i>executar uma instrução SQL</i> em tempo de execução.

Ao executar este código, será <b>gerada uma consulta SQL</b> do tipo:

<code>
	SELECT * FROM Clientes WHERE Nome = 'Yoda';
</code>
Assim, o programa pode <b>construir</b> consultas SQL personalizadas com base nos critérios escolhidos pelo <i>usuário, tornando a busca mais flexível e eficiente</i>.

### Overview: Storage Objects e SQL Dinâmico
Os <b>objetos de armazenamento</b> e <b>SQL dinâmico</b> são dois <i>conceitos diferentes, mas que podem estar relacionados</i> em alguns contextos.

Os objetos de armazenamento se <b>referem aos objetos</b> que armazenam dados em um banco de dados, como <i>tabelas, índices, views e procedimentos armazenados</i>. Esses objetos são <b>criados e gerenciados</b> através da linguagem SQL, que é a linguagem padrão para interagir com bancos de dados relacionais.

Já o SQL dinâmico é uma técnica que <b>permite a criação</b> de consultas SQL em tempo de execução, com base em parâmetros definidos pelo usuário. Isso pode ser útil em casos em que as consultas <i>precisam ser adaptadas de acordo</i> com as condições específicas de um determinado momento.

Em alguns casos, os objetos de armazenamento <i>podem ser usados</i> em conjunto com o SQL dinâmico, por exemplo, quando se deseja <b>criar uma consulta</b> que consulte uma tabela temporária criada em tempo de execução. Nesse caso, é possível criar a tabela temporária usando um objeto de armazenamento e, em seguida, <b>utilizar o SQL dinâmico</b> para criar a consulta que a utiliza.

Os <b>objetos de armazenamento e o SQL dinâmico</b> são conceitos distintos, mas que podem ser usados em conjunto para criar soluções mais flexíveis e adaptáveis em bancos de dados relacionais.

Além disso, o SQL dinâmico pode ser usado para <b>criar consultas</b> mais <i>complexas e personalizadas, que não podem ser facilmente criadas com as opções padrão do SQL</i>. Por exemplo, é possível criar uma consulta que retorne resultados diferentes com base em diferentes conjuntos de critérios de pesquisa, que podem ser <b>definidos pelo usuário</b> em <b>tempo de execução</b>.

No entanto, é importante lembrar que o <b>uso excessivo</b> do SQL dinâmico pode levar a <b>problemas de segurança</b>, como a injeção de SQL, que pode permitir que um atacante execute comandos maliciosos no banco de dados. Por isso, é <b>importante</b> garantir que as consultas dinâmicas sejam criadas de <i>forma segura e cuidadosa</i>, utilizando técnicas como a <i>validação de entrada de dados e a parametrização de consultas</i>.

Resumindo, os objetos de armazenamento e o SQL dinâmico são <b>dois conceitos importantes</b> no contexto de bancos de dados relacionais. Enquanto os objetos de armazenamento são usados para armazenar dados em tabelas e outros objetos de banco de dados, o SQL dinâmico permite a criação de consultas personalizadas em tempo de execução, o que pode ser útil para adaptar as consultas às condições específicas de um determinado momento.

### Statement de controle de fluxo
O controle de fluxo em SQL pode ser feito usando <b>declarações condicionais</b>, como <b>IF-ELSE, CASE-WHEN e WHILE</b>.

A <b>declaração IF-ELSE</b> é usada para executar um bloco de código se uma condição for <b>verdadeira</b> e outro bloco de código se a condição for <b>falsa</b>. Por exemplo:
<code>
IF condição THEN
   -- bloco de código a ser executado se a condição for verdadeira
ELSE
   -- bloco de código a ser executado se a condição for falsa
END IF;
</code>

A <b>declaração CASE-WHEN</b> é usada para <i>avaliar uma expressão e executar um bloco de código</i> correspondente com base no valor da expressão. Por exemplo:
<code>
CASE expressão
   WHEN valor1 THEN
      -- bloco de código a ser executado se a expressão for igual a valor1
   WHEN valor2 THEN
      -- bloco de código a ser executado se a expressão for igual a valor2
   ELSE
      -- bloco de código a ser executado se nenhum dos valores anteriores corresponder à expressão
END CASE;
</code>

A <b>declaração WHILE</b> é usada para executar um bloco de código repetidamente enquanto uma condição for <b>verdadeira</b>. Por exemplo:
<code>
WHILE condição LOOP
   -- bloco de código a ser executado enquanto a condição for verdadeira
END LOOP;
</code>
Essas declarações podem ser combinadas para criar <b>fluxos de controle (statement)</b> mais complexos em SQL.

### Condition Handling
A <b>manipulação de condições</b> em bancos de dados NoSQL pode variar dependendo do tipo de banco de dados NoSQL que está sendo utilizado. No entanto, em geral, os bancos de dados NoSQL <b>têm seus próprios</b> mecanismos de <b>manipulação de condições</b>.

Por exemplo, em bancos de dados NoSQL baseados em documentos, como o <b>MongoDB</b>, a <i>manipulação de condições é realizada usando a linguagem de consulta de documentos do MongoDB</i>, que inclui operadores de consulta, como <b>$eq (igual), $gt (maior que), $lt (menor que) e outros</b>. Esses operadores podem ser usados para filtrar documentos com base em <b>condições específicas</b>.

Já em bancos de dados NoSQL <b>baseados em chave-valor</b>, como o Redis, a <b>manipulação de condições</b> é feita por meio do uso de comandos específicos, como <b>ZRANGEBYSCORE</b> (para recuperar um intervalo de valores com base em uma pontuação) ou <b>HGETALL</b> (para recuperar todos os valores em um hash). Esses comandos podem ser usado para realizar <b>operações condicionais</b> em dados armazenados no Redis.

Em resumo, a manipulação de condições em bancos de dados NoSQL é geralmente <i>feita usando uma combinação de operadores de consulta ou comandos específicos</i> de banco de dados, dependendo do tipo de banco de dados NoSQL que está sendo utilizado.

### Storage Objects: FUNCTIONS, PROCEDURES e EVENTS
<b>Funções, procedimentos e eventos</b> são objetos de armazenamento comuns em bancos de dados SQL. No entanto, em bancos de dados NoSQL, a forma como esses objetos são implementados pode variar.

Em bancos de dados NoSQL baseados em documentos, como o MongoDB, as <i>funções são escritas em JavaScript e são usadas para realizar operações complexas nos documentos armazenados</i>. Os procedimentos armazenados são implementados como funções JavaScript armazenadas no servidor e podem ser chamados de forma síncrona ou assíncrona. <b>Events</b>, por sua vez, são <b>triggers</b> que disparam uma ação quando um determinado evento ocorre no banco de dados, <b>como a inserção</b> de um novo documento.

Já em bancos de dados NoSQL baseados em gráficos, como o Neo4j, <i>as funções são escritas em Cypher, a linguagem de consulta do Neo4j</i>. Os procedimentos são escritos em Java e podem ser chamados de forma síncrona ou assíncrona. Os eventos, chamados de triggers no Neo4j, são acionados <b>quando uma ação específica ocorre</b> no banco de dados, como a criação de um novo nó.

Em geral, esses objetos de armazenamento têm a função de <b>aumentar a eficiência e a funcionalidade</b> do banco de dados, permitindo que os usuários <i>escrevam código personalizado para manipular dados e responder</i> a eventos específicos.

### Exemplo de Função no MySQL
Em SQL, as <b>funções são usadas para executar</b> uma determinada tarefa ou operação e retornar um valor. Elas podem ser usadas em <b>consultas SELECT</b>, para <i>calcular valores, converter tipos de dados, manipular strings e datas, entre outras operações</i>.

Algumas <b>funções comuns</b> em SQL incluem:

<b>• Funções de agregação:</b> como SUM, AVG, COUNT, MAX e MIN, que são usadas para <i>realizar cálculos</i> em um conjunto de dados.
<b>• Funções de conversão de tipo:</b> como CAST e CONVERT, que são usadas para <i>converter um tipo</i> de dado em outro.
<b>• Funções de manipulação de strings:</b> como SUBSTRING, REPLACE e UPPER/LOWER, que são usadas para <i>manipular cadeias de caracteres</i>.
<b>• Funções de manipulação de datas:</b> como DATEADD, DATEDIFF e GETDATE, que são usadas para <i>manipular datas e horários</i>.

Ao usar <b>funções em SQL</b>, é possível <i>simplificar as consultas e automatizar tarefas repetitivas</i>.

A sintaxe básica para criar uma função no MySQL é a seguinte:
<code>
	CREATE FUNCTION nome_da_funcao (argumentos)
	RETURNS tipo_de_retorno
	BEGIN
    	-- Corpo da função
	END;
</code>

Onde:
<b>• nome_da_funcao:</b> é o nome que você deseja dar à sua função.
argumentos são os parâmetros que a função recebe. Você pode ter nenhum ou vários argumentos separados por vírgulas. Cada argumento tem um nome e um tipo.
<b>• tipo_de_retorno:</b> é o tipo de dado que a função retorna. Pode ser um tipo de dado nativo do MySQL (como INTEGER, VARCHAR, etc.) ou um tipo de dado definido pelo usuário.
<b>• BEGIN e END:</b> definem o corpo da função. É aqui que você escreve as instruções que a função executará.
Por exemplo, se você quiser criar uma <b>função que receba</b> dois números e retorne a soma deles, você pode usar o seguinte código:
<code>
	CREATE FUNCTION soma (a INT, b INT)
	RETURNS INT
	BEGIN
    	RETURN a + b;
	END;
</code>

Depois de criar a função, você pode usá-la como <i>qualquer outra função</i> no MySQL. Por exemplo:
<code>
	SELECT soma(2, 3); -- retorna 5
</code>

Dentro do <b>corpo da função</b>, você pode escrever qualquer código SQL que seja válido no MySQL. Você pode usar instruções <b>SELECT, UPDATE, INSERT, DELETE, IF, WHILE, entre outras</b>.

Além disso, você pode declarar variáveis dentro da função usando a <b>palavra-chave DECLARE</b>, como no exemplo abaixo:
<code>
	CREATE FUNCTION calcula_salario (salario_base DECIMAL(10,2), horas_trabalhadas INT)
	RETURNS DECIMAL(10,2)
	BEGIN
    	DECLARE salario_total DECIMAL(10,2);
    	SET salario_total = salario_base * horas_trabalhadas;
    	RETURN salario_total;
	END;
</code>
Neste exemplo, a <b>função calcula</b> o salário total de um funcionário com <i>base no salário base e no número de horas trabalhadas</i>. A função declara a variável <b>"salario_total"</b> usando a <b>palavra-chave DECLARE</b> e, em seguida, a popula com o valor calculado na linha seguinte usando a instrução <b>SET</b>. Finalmente, a função <b>retorna o valor</b> da variável <b>"salario_total"</b>.

Uma vez que a função tenha sido criada, você pode chamá-la em <b>qualquer lugar</b> em que seria apropriado chamar uma função no MySQL. Por exemplo:
<code>
	SELECT calcula_salario(1000.00, 160); -- retorna 160000.00
</code>

### Exemplo de Precedure no MySQL
Em SQL, uma <b>procedure (procedimento armazenado)</b> é um bloco de código SQL que é armazenado no banco de dados e pode ser <i>chamado e executado várias vezes</i>. Elas são usadas para <i>automatizar tarefas complexas e repetitivas</i> que envolvem várias etapas ou consultas SQL.

As procedures podem receber parâmetros de <b>entrada e de saída</b> e são especialmente úteis para <b>realizar operações complexas</b> que envolvem várias <i>consultas SQL e lógica de programação</i>. Por exemplo, uma procedure pode ser criada para <b>calcular uma média</b> ponderada de um <i>conjunto de dados, realizar uma atualização em massa de uma tabela ou gerar um relatório complexo</i>.

Algumas <b>vantagens</b> do uso de procedures em SQL incluem:

<b>• Redução da complexidade da lógica de programação:</b> pois as tarefas complexas podem ser divididas em etapas menores e mais gerenciáveis.
<b>• Maior desempenho:</b> pois as procedures são compiladas e armazenadas no banco de dados, o que reduz o tempo de execução.
<b>• Maior segurança:</b> pois as procedures podem ser definidas com permissões de acesso restritas para garantir a segurança dos dados do banco.
As procedures são uma ferramenta útil para <i>simplificar e automatizar</i> tarefas complexas em SQL.

Segue abaixo um exemplo de criação de uma procedure no MySQL:
<code>
CREATE PROCEDURE nome_da_procedure (IN parametro1 INT, IN parametro2 VARCHAR(50))
BEGIN
   -- Corpo da procedure aqui
END;
</code>

Neste exemplo, é criada uma procedure chamada <b>"nome_da_procedure"</b> com dois parâmetros de entrada: um inteiro chamado <b>"parametro1"</b> e uma string de até 50 caracteres chamada <b>"parametro2"</b>. O corpo da procedure deve ser definido dentro do <b>bloco BEGIN e END</b>, e pode conter <b>uma ou mais</b> instruções SQL.

<code>
CREATE PROCEDURE sp_insere_cliente (IN nome VARCHAR(50), IN email VARCHAR(100))
BEGIN
   INSERT INTO clientes (nome, email) VALUES (nome, email);
END;
</code>

Neste exemplo, é criada uma procedure chamada <b>"sp_insere_cliente"</b> que insere um novo registro na tabela <b>"clientes"</b> do banco de dados. A procedure <b>recebe dois parâmetros</b> de entrada: um string chamado <b>"nome"</b> e uma string chamada <b>"email"</b>. Na instrução <b>INSERT INTO</b>, os valores dos parâmetros são usados para <b>inserir um novo</b> registro na tabela.

Para <b>chamar</b> essa procedure, basta utilizar o comando <b>CALL</b> seguido do <b>nome da procedure</b> e dos <b>valores dos parâmetros</b>:
<code>
CALL sp_insere_cliente('Naymar', 'neymar@corinthians.com.br');
</code>

Esse comando vai <b>inserir</b> um novo registro na tabela <b>"clientes"</b> com os valores "Neymar" e "neymar@corinthians.com.br" nas colunas <b>"nome"</b> e <b>"email"</b>.

## Overview sobre Automação de Ações com Triggers no MySQL
A <b>automação de ações com triggers</b> no MySQL é uma funcionalidade muito útil que <i>permite automatizar tarefas</i> em um banco de dados, tornando o processo de gerenciamento de dados mais <b>eficiente e fácil</b>.

As triggers são procedimentos armazenados que são <b>executados automaticamente</b> quando um determinado evento ocorre no banco de dados, como a <i>inserção, atualização ou exclusão</i> de registros em uma tabela. Com as triggers, é possível definir ações que serão executadas automaticamente em resposta a um determinado evento, como a <i>atualização de um registro</i> em uma tabela.

Por exemplo, se você deseja <b>atualizar um campo</b> em uma tabela sempre que <i>outro campo for atualizado</i>, você pode criar uma trigger que <b>execute automaticamente</b> a atualização do campo. Isso <i>elimina a necessidade de atualizar</i> o campo manualmente toda vez que o outro campo é atualizado.

As triggers também podem ser usadas para <i>validar dados, garantir a integridade referencial e implementar restrições de segurança</i>. Por exemplo, você pode usar uma trigger para <b>garantir</b> que um valor inserido em uma tabela <i>esteja dentro</i> de um intervalo específico, ou para impedir que um registro <i>seja excluído</i> de uma tabela se ele estiver relacionado a outros registros em outras tabelas.

A automação de ações com triggers no MySQL é uma <b>funcionalidade poderosa</b> que pode tornar o gerenciamento de dados <b>mais eficiente e fácil</b>. É importante ter um bom <b>entendimento da sintaxe</b> e do funcionamento das triggers antes de implementá-las em seu banco de dados.

Além disso, é importante destacar que as triggers <b>podem ter impacto</b> no desempenho do banco de dados, especialmente se forem mal projetadas ou usadas de <b>forma inadequada</b>. Por isso, é importante levar em consideração as melhores práticas ao usar triggers, como <i>limitar o número de triggers em uma tabela e otimizar a lógica da trigger</i> para evitar operações desnecessárias.

Outro ponto <b>importante</b> é que as triggers podem ser usadas em <b>conjunto</b> com outras funcionalidades do MySQL, como <i>stored procedures e views</i>, para criar soluções mais <i>avançadas e automatizadas</i> de gerenciamento de dados. Por exemplo, você pode criar uma trigger que chama uma stored procedure sempre que um <b>determinado evento ocorre</b> no banco de dados.

Resumindo o que foi falado, a automação de ações com triggers no MySQL é uma <b>funcionalidade poderosa</b> que pode tornar o gerenciamento de dados <b>mais eficiente e fácil</b>, mas que também <b>requer cuidado e atenção</b> ao ser implementada. Com as melhores práticas e a compreensão adequada da sintaxe e do funcionamento das triggers, é possível criar soluções <i>avançadas e automatizadas</i> de gerenciamento de dados no MySQL.

### Assertions e Triggers
<b>• Aassertions:</b> são <b>condições declarativas</b> que <i>especificam restrições sobre os dados em uma tabela</i>. Elas permitem que você <b>defina regras</b> complexas de integridade de dados que vão além das verificações simples de <b>chave primária ou estrangeira</b>. As <b>"assertions"</b> são usadas para garantir que os dados armazenados em uma tabela estejam sempre em um estado consistente.

<b>• Triggers:</b> são <b>rotinas</b> que são automaticamente executadas em resposta a determinados eventos, como a <i>inserção, atualização ou exclusão</i> de dados em uma tabela. Eles permitem que você defina ações personalizadas que devem ser executadas sempre que um evento específico ocorrer. Os <i>"triggers"</i> podem ser usados para <i>implementar regras de negócios complexas ou para manter a integridade dos dados</i>.

Em resumo, as "assertions" são usadas para <b>definir restrições</b> declarativas sobre os dados em uma tabela, enquanto os "triggers" são usados para <b>executar ações personalizadas</b> em resposta a eventos específicos. Ambos são recursos poderosos do SQL que permitem que você crie sistemas de banco de dados mais <i>robustos e confiáveis</i>.

### Funcionamento de Assertions
Assertions são <b>declarações que especificam condições</b> que devem ser <B>verdadeiras</B> após a conclusão de uma transação. As assertions são usadas para <i>garantir que o estado</i> do banco de dados <i>esteja sempre em conformidade</i> com certas restrições.

As assertions são <b>semelhantes às restrições</b>, mas <b>diferem no momento</b> em que são verificadas. As restrições são verificadas durante as operações de <i>inserção, atualização ou exclusão</i> de dados, enquanto as assertions são <b>verificadas após a conclusão</b> de uma transação.

As assertions são criadas usando a <b>cláusula CREATE ASSERTION</b>, seguida de uma <i>expressão booleana que deve ser verdadeira</i> após a conclusão de uma transação. Por exemplo, a seguinte assertion garante que o preço dos produtos nunca seja negativo:
<code>
CREATE ASSERTION preço_não_negativo
CHECK (NOT EXISTS (SELECT * FROM produtos WHERE preço < 0));
</code>

Se uma transação <b>violar</b> uma assertion, a transação será <b>revertida</b> e um <i>erro será gerado</i>. As assertions são <b>úteis para garantir</b> que o banco de dados esteja sempre em um estado consistente e para <b>evitar</b> que <i>dados inválidos sejam inseridos</i> no banco de dados.

### Especificando Constraints com Triggers
Os triggers são <b>objetos executados automaticamente</b> quando ocorre um evento específico, como uma <i>inserção, atualização ou exclusão</i> de dados de uma tabela. Eles podem ser usados para especificar <b>constraints adicionais</b> em uma tabela, além das que foram definidas quando a tabela foi criada.

Por exemplo, suponha que você tenha uma tabela <b>"Funcionários"</b> com uma coluna <b>"Salário"</b> e que queira garantir que nenhum funcionário receba um salário <b>abaixo do mínimo legal</b>. Você pode definir uma <b>constraint CHECK</b> na criação da tabela para garantir isso. No entanto, se você quiser ter certeza de que essa constraint é sempre respeitada, mesmo se alguém <i>atualizar a tabela manualmente</i>, você pode criar um <b>trigger AFTER UPDATE</b> que verifique se o salário atualizado <i>respeita a constraint</i>.

Outro exemplo seria uma <b>tabela de pedidos</b>, em que você deseja garantir que a quantidade de itens em um pedido <b>não seja maior</b> do que o estoque disponível. Neste caso, você pode criar um <b>trigger BEFORE INSERT</b> que verifique se a quantidade de itens solicitados não excede o estoque disponível <b>antes de permitir</b> que o pedido seja adicionado à tabela.

Os triggers podem ser usados para <b>complementar as constraints</b> existentes em uma tabela e <b>garantir</b> que os dados permaneçam consistentes, <b>mesmo quando são modificados</b> fora do controle do aplicativo.

### Exemplo de Trigger BEFORE INSERT no MySQL
Suponha que temos uma tabela chamada <b>"clientes"</b> com as seguintes colunas: <b>"id", "nome", "email" e "telefone"</b>. Queremos que, antes de um <i>novo registro ser inserido</i> na tabela <b>"clientes"</b>, seja verificado se o email já existe na tabela. Se existir, a inserção deve ser cancelada e uma mensagem de erro deve ser exibida.

Para isso, podemos criar o seguinte Trigger:
<code>
	CREATE TRIGGER antes_de_inserir_cliente
	BEFORE INSERT ON clientes
	FOR EACH ROW
	BEGIN
  	IF EXISTS (SELECT * FROM clientes WHERE email = NEW.email) THEN
    	SIGNAL SQLSTATE '45000' 
      	SET MESSAGE_TEXT = 'Já existe um cliente cadastrado com esse e-mail.';
  	END IF;
END;
</code>

<b>• antes_de_inserir_cliente</b> é o nome do Trigger que estamos criando.
<b>• BEFORE INSERT</b> indica que o Trigger será executado antes de um novo registro ser inserido na tabela "clientes".
<br>
<b>• FOR EACH ROW</b> indica que o Trigger será executado para cada linha que for inserida na tabela.
<br>
<b>• IF EXISTS</b> verifica se já existe um registro na tabela com o email que está sendo inserido (usando a variável NEW.email, que representa o valor que será inserido na coluna "email").
<br>
<b>• SIGNAL SQLSTATE '45000' SET MESSAGE_TEXT = </b> é uma forma de gerar um erro personalizado. O código SQLSTATE '45000' indica que ocorreu um erro definido pelo usuário, e a mensagem de erro será 'Já existe um cliente cadastrado com esse e-mail.'.
Dessa forma, se alguém tentar inserir um novo registro na tabela "clientes" com um email que já existe, o Trigger será acionado e a inserção será cancelada, exibindo a mensagem de erro <b>'Já existe um cliente cadastrado com esse e-mail.'</b>.

### Exemplo de Trigger AFTER INSERT no MySQL
Suponha que você tenha uma tabela chamada <b>"clientes"</b> e queira criar uma tabela de histórico para <b>armazenar as informações</b> de cada cliente que é <b>inserido</b> na tabela principal. O código abaixo mostra <i>como criar um trigger que insere os dados</i> do cliente na tabela de histórico após uma <b>inserção</b> na tabela principal:
<code>
CREATE TRIGGER insere_historico_cliente AFTER INSERT ON clientes
FOR EACH ROW
BEGIN
    INSERT INTO historico_clientes (id_cliente, nome, email, telefone, data_cadastro)
    VALUES (NEW.id, NEW.nome, NEW.email, NEW.telefone, NOW());
END;
</code>

O trigger é criado com o nome <b>"insere_historico_cliente"</b> e é definido para executar <b>AFTER INSERT</b> na tabela <b>"clientes"</b>. A cláusula <b>FOR EACH ROW</b> indica que o trigger deve ser <i>executado para cada linha que é inserida</i> na tabela.

Dentro do corpo do trigger, a cláusula <b>BEGIN</b> e <b>END</b> é usada para agrupar as instruções a serem executadas pelo trigger. A instrução <b>INSERT INTO</b> é usada para inserir os dados do cliente na tabela de <b>histórico_clientes</b>. Os valores são obtidos a partir da <b>palavra-chave "NEW"</b>, que é uma referência à linha recém-inserida na tabela <b>"clientes"</b>. A data atual é adicionada à coluna <b>data_cadastro</b> usando a função <b>NOW()</b>.

### Exemplo de Gatilho BEFORE UPDATE TRIGGER no MySQL
Suponha que temos a tabela <b>"clientes"</b> com as colunas <b>"id", "nome", "email" e "idade"</b>. Desejamos que a idade do cliente <b>nunca seja menor do que zero</b>. Para isso, podemos criar o seguinte trigger:
<code>
CREATE TRIGGER antes_atualizar_cliente
BEFORE UPDATE ON clientes
FOR EACH ROW
BEGIN
    IF NEW.idade < 0 THEN
        SIGNAL SQLSTATE '45000' SET MESSAGE_TEXT = 'A idade não pode ser negativa';
    END IF;
END;
</code>

Neste exemplo, o trigger é criado com o nome <b>"antes_atualizar_cliente"</b> e é acionado antes de uma <b>atualização (UPDATE)</b> ser feita na tabela <b>"clientes"</b>. A <b>condição IF</b> verifica se o novo valor da coluna <b>"idade"</b> é menor do que zero. Se isso for verdadeiro, o <b>sinalizador (SIGNAL)</b> é acionado, com a mensagem de erro <b>'A idade não pode ser negativa'</b>.

Dessa forma, se alguém tentar atualizar a idade de um cliente para um <b>valor negativo</b>, o trigger irá <b>impedir</b> a atualização e exibirá a mensagem de erro <b>'A idade não pode ser negativa'</b>.


<br><br><br>
Agradecimentos a <a href="https://dio.me">DIO - Digital Inovation One</a> pelo conhecimento

