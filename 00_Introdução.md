##Introdução
No mundo atual existem gigantescos bancos de dados
gerenciando nossas vidas. Nossa conta bancária faz parte de uma
coleção imensa de contas bancárias de nosso banco. Nosso Título
Eleitoral ou nosso Cadastro de Pessoa Física, certamente estão
armazenados em Bancos de Dados colossais. Sabemos também
que quando sacamos dinheiro no caixa eletrônico de nosso banco,
nosso saldo e as movimentações existentes em nossa conta
bancária já estão à nossa disposição.
Nestas situações sabemos que existe uma necessidade em
se realizar o armazenamento de uma série de informações que
não se encontram efetivamente isoladas umas das outras, ou seja,
existe uma ampla gama de dados que se referem a relacionamentos
existentes entre as informações a serem manipuladas.
Para gerenciar tantos dados como os citados são utilizados
os Sistemas de Gerenciamento de Banco de Dados (SGBD).
Sem tais sistemas o mundo atual estaria bastante diferente de como vemos hoje. O mercado financeiro tal como vemos hoje não
existiria. As praticidades como compras pela Internet, cartões de débito, caixas automáticos e mais uma infinidade de exemplos
não seriam possíveis.

### Popularização dos Bancos de Dados.

   Há poucas décadas atrás os bancos de dados eram utilizados
apenas por grandes instituições, e seu uso era restrito aos grandes negócios, onde simplesmente seria impossível a operação de certas indústrias ou empresas.
   Com a popularização e barateamento da plataforma IBM/PC,
logo surgiram programas aplicativos para algum tipo de
armazenamento de dados.
   Antes desses equipamentos e softwares tornarem-se
acessíveis muitas vezes eram utilizadas fichas cadastrais para
armazenar dados de clientes em pequenos e médios negócios
(essas fichas e armários de fichários são ainda hoje utilizados em
alguns locais).
   Para se entender como isso funcionava vamos usar um
exemplo de uma pessoa que ao visitar uma clínica médica/
odontológica fornecia seu nome, endereço, telefone, etc. Esses
dados eram então anotados nessas fichas, que eram a maneira de
se guardar as informações de clientes, pacientes, estudantes, peças numa oficina mecânica, etc..

**Exemplo de ficha cadastral:**
![](https://i.imgur.com/Sj7yL8T.png)

Quando era necessário saber o número de telefone de um
cliente chamado "Raoni Guimarães Villar de Pinho" era preciso
abrir o fichário, encontrar a letra R e ir olhando aos poucos onde havia o nome Raoni. Se fosse preciso saber, em uma escola, se o aluno "Artur Magno Horta de Abreu" havia repetido alguma série, era preciso verificar as fichas que continham os históricos escolares, depois procurar pelo histórico do aluno e ainda procurar nessa ficha se o aluno havia repetido alguma série. No caso de uma farmácia, saber quais produtos custavam mais que R$ 5,00 seria extremamente difícil, e nada disso era feito.
Atualmente os bancos de dados estão por toda parte, desde a
farmácia da esquina até a lojinha do posto de gasolina.


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

Exemplo de uma tabela de um Banco de Dados Relacional: