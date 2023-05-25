# SQL

### INTRODUÇÃO

Para se utilizar, administrar, e trabalhar com um banco de
dados é utilizada uma linguagem padrão, que a maior parte dos
SGBD aceitam. Essa linguagem é a SQL (Structured Query
Language-Linguagem de Consulta Estruturada).

A SQL é um conjunto de declarações que são utilizadas para
acessar os dados utilizando gerenciadores de banco de dados.
Apesar de nem todos os gerenciadores utilizarem a SQL a maior
parte deles aceitam suas declarações.
A SQL pode ser utilizada para todas as atividades relativas a
um banco de dados, podendo ser utilizada pelo administrador de
sistemas, pelo DBA, por programadores, sistemas de suporte à
tomada de decisões e outros usuários finais.
É através dela que você irá criar tabelas, inserir dados, e utilizar
o seu banco de dados.


### SQL para manipulação de bancos de dados MySQL

A SQL possui comandos que são utilizados para manipular os
bancos de dados, as tabelas e os registros existentes. Veja abaixo
como utilizá-los.

**COMANDO CREATE** --> Este comando permite a criação de bancos de dados ou de
tabelas num banco de dados.

Sintaxe:
**CREATE DATABASE** < nome_db >;
onde:
**nome_db**: indica o nome do Banco de Dados a ser criado.

Exemplo:
**CREATE DATABASE** curso;

Sintaxe:

**CREATE TABLE** < nome_tabela > (
nome_atributo1 < tipo > [ NOT NULL ],
nome_atributo2 < tipo > [ NOT NULL ],
 ......
nome_atributoN < tipo > [ NOT NULL ]
**PRIMARY KEY**(nome_atributo)
) ;

onde:
nome_tabela: indica o nome da tabela a ser criada.
nome_atributo: indica o nome do campo a ser criado na tabela.
tipo: indica a definição do tipo de atributo ( integer(n), char(n),
... ).

**PRIMARY KEY**: esse é o campo utilizado para que não exista
na tabela dois registros iguais. Ele mantém a integridade do banco
de dados. Caso você tente inserir num banco de dados um registro
com uma **PRIMARY KEY** já existente ele emitirá uma mensagem
de erro e impedirá que o registro seja inserido.

Exemplo:
**CREATE table** alunos(
codigo int NOT NULL AUTO_INCREMENT,
nome VARCHAR(20) NOT NULL ,
telefone CHAR(8) NOT NULL,
PRIMARY KEY(codigo)
);
Criação de uma tabela em um banco de dados à partir da
tabela dada (o asterísco determina qual campo é a chave primária):

![](https://i.imgur.com/aOc0xXK.png)

**CREATE TABLE** estudantes(
numerocadastro int NOT NULL auto_increment,
nome varchar(35) not null,
turma int,
primary key(numerocadastro)
);

**COMANDO DROP**
Este comando elimina a definição da tabela, seus dados e
referências ou um banco de dados existente:

Sintaxe:

DROP TABLE < nome_tabela > ;
<br>
DROP DATABASE <nome_banco_de_dados>;

Exemplo:
DROP TABLE alunos; <br>
DROP DATABASE curso;<br>
DROP TABLE estudantes;



