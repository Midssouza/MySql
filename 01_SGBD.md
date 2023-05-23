### Sistema de Gerenciamento de Banco de Dados?

Um SGBD - Sistema de Gerenciamento de Banco de Dados é
uma coleção de programas que permitem ao usuário definir,
construir e manipular Bancos de Dados para as mais diversas
finalidades.
Um SGBD deve possuir as seguintes características:

###### CONTROLE DE REDUNDÂNCIAS

A redundância consiste no armazenamento de uma mesma
informação em locais diferentes, provocando inconsistências. Em
um Banco de Dados as informações só se encontram armazenadas
em um único local, não existindo duplicação descontrolada dos
dados. Quando existem replicações dos dados, estas são
decorrentes do processo de armazenagem típica do ambiente
Cliente-Servidor, totalmente sob controle do Banco de Dados.

###### COMPARTILHAMENTO DOS DADOS

O SGBD deve incluir software de controle de concorrência ao
acesso dos dados, garantindo em qualquer tipo de situação a escrita/leitura de dados sem erros.

###### CONTROLE DE ACESSO.

O SGDB deve dispor de recursos que possibilitem selecionar
a autoridade de cada usuário. Assim um usuário poderá realizar
qualquer tipo de acesso, outros poderão ler alguns dados e atualizar outros e outros ainda poderão somente acessar um conjunto restrito de dados para escrita e leitura.

###### INTERFACEAMENTO

Um Banco de Dados deverá disponibilizar formas de acesso
gráfico, em linguagem natural, em SQL ou ainda via menus de
acesso, não sendo uma "caixa-preta" somente sendo passível de
ser acessada por aplicações.

###### ESQUEMATIZAÇÃO

Um Banco de Dados deverá fornecer mecanismos que
possibilitem a compreensão do relacionamento existentes entre
as tabelas e de sua eventual manutenção.

###### CONTROLE DE INTEGRIDADE
Um Banco de Dados deverá impedir que aplicações ou
acessos pelas interfaces possam comprometer a integridade dos
dados.

###### CÓPIAS DE SEGURANÇA
O SGBD deverá apresentar facilidade para recuperar falhas
de hardware e software, através da existência de arquivos de "préimagem" ou de outros recursos automáticos, exigindo
minimamente a intervenção de pessoal técnico.
Em certos casos pode ocorrer de um SGBD não obedecer
uma ou outra regra das vistas acima, mas ainda assim continuar
sendo considerado um SGBD. Porém alguns "Bancos de Dados"
atualmente comercializados não são SGBD reais, justamente por
não atenderem algumas dessas características.
Existem vários tipos de bancos de dados (hierárquico,
orientado ao objeto, em redes), nós utilizaremos nesse curso um
SGBD Relacional, o MySQL.

**Exemplo de uma tabela de um Banco de Dados Relacional:**

![](https://i.imgur.com/zHEExYY.png)
