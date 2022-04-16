<div align=center>
  <img src="brasaooficialcolorido.png">
</div>

#### <p style="text-align: center;">Universidade Federal de Goiás</p>
#### <p style="text-align: center;">Instituto de Informática</p>
#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P2 - 12/04/2022</p>

Matrícula: 201902769

Nome: Jacob Ferraz dos Santos

<font color="red">Nota 1,24</font>

1. Quanto ao Processo de Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Defina os seguintes conceitos Processo de Teste de Software, Projeto de Teste de Software e Plano de Teste de Sofware.
   2. (**0,5 ponto**) Descreva o relacionamento existente entre estes conceitos.
2. (**1,0 pontos**) Descreva as vantagens para a equipe de desenvolvimento ao se adotar um processo de teste ágil.
3. (**1,0 ponto**) Cite pelo menos três características do Teste Exploratório.
4. Considere os arquivos .java (Banco.java, Agencia.java, Conta.java e BankValidator.java). Nos próprios arquivos .java estão definidas as regras para cadastramento de cada um deles (Banco, Agencia e Conta). Desta forma, pede-se:
   1. (2.0 Pontos) Definir os cenários de teste suficientes para testar o cadastro e movimentações financeiras envolvendo bancos, agências e contas, conforme especificado. Para cada cenário definir os critérios de teste adequados à definição dos seus casos de teste.
   2. (2.0) Definir os casos de teste suficientes para a cobertura do teste de cada um dos cenários definidos. Documentar os casos de teste no seguinte padrão:
   |CT|Valores de Entrada|Resultado esperado|
   |---|---|---|
   |||
   3. (3.0 Pontos) Implementar (na linguagem de programação java) as classes para o teste da criação dos objetos e das movimentações financeiras envolvendo bancos e agências e contas.

   <font color="red">Nota 1,24</font>

INSTRUÇÕES:
1. Tipo: Prova individual;
2. Local de Entrega: Plataforma Turing.
3. Forma de Entrega: arquivo compactado contendo:
   1. Este arquivo md, respondido.
   2. Classes de teste para (BancoTest, AgenciaTest e ContaTest);
   3. O arquivo compactado deverá ter o seguinte nome prova_p2<mat>.zip, onde mat é o número da matrícula do aluno(a).
5. Data da Entrega: 12/04/2022, as 22hs.
6. Critério de Aceitação: arquivo entregue, conforme solicitado.
7. Obs: segue no mesmo pacote o arquivo "org.apache.commons.lang.StringUtils", que é uma dependência do projeto. É deve ser inserida no _classpath_ do projeto de implementação da questão 4, caso não esteja utilizando o _maven_.

**RESPOSTAS**

1.

    1.1
O Processo de Teste de Software tem como principal objetivo estruturar as etapas, as atividades, os artefatos, os papéis, e as responsabilidades dos testes, criando um processo organizacional de todo o ciclo do teste.
O Projeto de Testes informa a estrutura dos elementos de testes e a relização dos casos de teste.
Já o Plano de Teste é um documento que demonstra em uma abordagem sistemática para os testes, modelando detalhadamente o fluxo de trabalho de testes do processo de teste.

    1.2
O Processo de Teste estrutura como os testes deveram ser organizados, estruturados e quais suas responsabilidades, o projeto de teste informa como será feita a implementação do processo de teste, e o plano informa sistematicamente como o projeto de teste será executado.

2.

A atividade de teste no processo de teste ágil é realizada em todas as fases do projeto, onde todos os profissionais envolvidos no ciclo de vida do software participam da garantia da qualidade, logo temos que a responsabilidade da qualidade passa a ser de toda a equipe, integrando diversas áreas focando em construir o software bem feito, em vez de construir e depois encontrar defeitos, assim o sistema já nasce sendo pensado na qualidade, diminuindo o retrabalho e a quantidade de defeitos, assim como, o time inteiro participa ativamente da qualidade, gerando um fluxo ágil dentro do processo de teste.

3.

Os resultados dos testes, casos de testes e documentação de testes são geradas a medida que os testes são realizados.
Os testadores podem interagir com a aplicação da forma como quiserem e usar as informações obtidas para, reagir, alterar o curso e explorar funcionalidades da aplicação sem repressão.
Com a falta de preparação, estrutura e diretrizes podem levar a improdutividade e reteste da mesma funcionalidade várias vezes.

4.

    4.1

Cénarios de Teste Agencia

| Código | Descrição| Resultado |
| -------- | -------- | -------- |
| CET1| Nome possuir 4 caracteres | Inválido|
| CET2| Nome possuir 5 caracteres | Válido|
| CET3| Nome possuir 100 caracteres | Válido|
| CET4| Nome possuir 101 caracteres | Inválido|
| CET5| Nome possuir apenas letras | Válido|
| CET6| Nome possuir caracteres alfanumericos | Iválido|
| CET7| Cidade possuir 4 caracteres | Inválido|
| CET8| Cidade possuir 5 caracteres | Válido|
| CET9| Cidade possuir 100 caracteres | Válido|
| CET10| Cidade possuir 101 caracteres | Inválido|
| CET11| Cidade possuir apenas letras | Válido|
| CET12| Cidade possuir caracteres alfanumericos | Iválido|
| CET13| Numero possuir 6 digitos | Iválido|
| CET14| Numero possuir 3 digitos | Válido|
| CET15| Numero possuir 2 digitos | Iválido|

Cénarios de Teste Banco

| Código | Descrição| Resultado |
| -------- | -------- | -------- |
| CET16| Nome possuir 4 caracteres | Inválido|
| CET17| Nome possuir 5 caracteres | Válido|
| CET18| Nome possuir 100 caracteres | Válido|
| CET19| Nome possuir 101 caracteres | Inválido|
| CET20| Nome possuir apenas letras | Válido|
| CET21| Nome possuir caracteres alfanumericos | Iválido|
| CET22| Numero possuir 3 digitos | Válido|
| CET23| Numero possuir 4 digitos | Iválido|
| CET24| Numero ser maior que 0 | Válido|
| CET25| Numero ser menor que 0 | Inválido|

Cénarios de Teste Conta

| Código | Descrição| Resultado |
| -------- | -------- | -------- |
| CET26| Cidade possuir apenas letras | Válido|
| CET27| Cidade possuir caracteres alfanumericos | Iválido|
| CET28| Numero possuir 6 digitos | Válido|
| CET29| Numero possuir 3 digitos | Iválido|
| CET30| Numero possuir 7 digitos | Iválido|
| CET31| Tipo Corrente | Válido|
| CET32| Tipo Poupanca | Válido|
| CET33| Tipo Salario | Iválido|
| CET34| Tipo Corrente e Cheque Especial | Válido|
| CET34| Tipo Poupanca e Cheque Especial | Inválido|
| CET35| Saldo < 0 | Iválido|
| CET36| Saldo > 0 | Válido|
| CET37| Depositar > 0 | Válido|
| CET38| Depositar < 0 | Iválido|
| CET39| Transferir > 0 | Válido|
| CET40| Transferir < 0 | Iválido|
| CET41| Debitar Juros Cheque Especial > 0 | Válido|
| CET42| Debitar Juros Cheque Especial < 0 |Iválido|

    4.2

Os casos de Teste Equivalem a numeração especifica dos cenarios de testes, exemplo, CT1 equivale a CET1.

| CT   | Valores de Entrada       | Resultado esperado |
| ---- | ------------------------ | ------------------ |
| CT1  | Nome = JACO              | false              |
| CT2  | Nome = JACOB             | true               |
| CT3  | Nome = "JACOADADASD...." | true               |
| CT4  | Nome = "JACOBXVDSF...."  | false              |
| CT5  | Nome = "Jacob"           | true               |
| CT6  | Nome = "JACOB1"          | false              |
| CT7  | Cidade = "GOia"          | false              |
| CT8  | Cidade = "Goias"         | true               |
| CT9  | Cidade = "GOIAS....."    | false              |
| CT10 | Cidade = "Goias....."    | false              |
| CT11 | Cidade = "Goias"         | true               |
| CT12 | Cidade = "Goias12"       | false              |
| CT13 | Numero = 123456          | false              |
| CT14 | Numero = 123             | true               |
| CT15 | Numero = 12              | false              |
| CT16 | Nome = "Brad"            | false              |
| CT17 | Nome = "BRADE"           | true               |
| CT18 | Nome = "BR...."          | false              |
| CT19 | Nome = "BAR...."         | true               |
| CT20 | Nome = "BRADESCO"        | true               |
| CT21 | Nome = "BRASC12"         | false              |
| CT22 | Numero = 123             | true               |
| CT23 | Numero = 1234            | false              |
| CT24 | Numero = 123             | true               |
| CT25 | Numero = -123            | false              |
| CT26 | Cidade = "Goias"         | true               |
| CT27 | Cidade = "Goias12"       | False              |
| CT28 | Numero = 123456          | true               |
| CT29 | Numero = 123             | false              |
| CT30 | Numero = 1234567         | true               |
| CT31 | Tipo = "Corrente"        | true               |
| CT32 | Tipo = "Poupanca"        | true               |
| CT33 | Tipo = "Salario"         | false              |
| CT34 | Tipo = "Corrente"        | Limite > 0         |
| CT35 | Tipo =    "Poupanca"     | Limite = 0         |
| CT36 | Saldo < 0                | false              |
| CT37 | Saldo > 0                | true               |
| CT38 | Depositar = 15           | true               |
| CT39 | Depositar = -15          | false              |
| CT40 | Transferir = 15          | true               |
| CT41 | Transferir = -15         | false              |
| CT42 | Debitar Juros = 15       | true               |
