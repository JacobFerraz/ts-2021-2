<div align=center>
  <img src="https://i.imgur.com/39XdXEr.png">
</div>

#### <p style="text-align: center;">Universidade Federal de Goiás</p>
#### <p style="text-align: center;">Instituto de Informática</p>
#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P1 - 16/02/2022</p>

Matrícula: 201802769
Nome: Jacob Ferraz dos Santos

<p><font color=green>Nota: 8,6.</font></p>

1. Quanto ao objetivo do Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Qual o objetivo primário da atividade de teste de software?
   **R**: O principal objetivo do teste é identificar defeitos e problemas nos softwares para evitar que tais defeitos vazem durante o desenvolvimento e produção, reduzindo os custos fora de orçamento. <font color=orange>Parcialmente correte. Nota 0,25.</font>
   2. (**0,5 ponto**) O que acontece, quando não se atinge este objetivo primário?
   **R**: Quando os defeitos não são encontrados nas fases iniciais do desenvolvimento de software, eles tendem a se tornar mais difíceis de  serem corrigidos, principalmente quando o sistema entra em produção, acarretando em altos custos de refatoração e correção, quebrando por muitas vezes o orçamento planejado para o sistema. <font color=red>Errado.</font>

2. (**1,0 ponto**) Explique o que é o teste exaustivo e porque sua execução não é possível.
**R**:
No teste exaustivo, todas as possibilidades são testadas, ou seja, todas as entradas possíveis devem ser especificadas, para validar 100% que tal funcionalidade não possui defeitos, contudo, na maioria dos casos a execução do teste exaustivo é inviável, devido a quantidade de tempo necessário para sua execução e, em muitos casos é impossível, como por exemplo, realizar um teste exaustivo em um campo do tipo double, requer testar milhões de valores, já que o tipo double possui 10 bits de precisão, logo testar apenas os valores limites especificados se torna mais dinâmico e prático. <font color=green>Certo.</font>
3. (**1,0 ponto**) Cite pelo menos duas limitações da Técnica de Teste Funcional e duas da Técnica de Teste Estrutural.
**R**: Os testes estruturais, possuem algumas limitações, defeitos podem existir mesmo que o fluxo de controle esteja correto, com isso as saídas esperadas que verificam a existência de defeitos, e módulos de código podem executar corretamente diversos fluxos e falhar apenas para alguns específicos, contudo, os testes estruturais são de suma importância pois são complementares aos testes funcionais.
Já os testes funcionais também possuem algumas desvantagens, primeiramente eles são extremamente dependentes das especificações de requisitos, que na maioria dos casos não é bem feita, não é possível garantir que partes essenciais do software sejam executadas e testadas, e por fim, para encontrar todos os possíveis defeitos utilizando testes funcionais, é necessário utilizar o teste exaustivo, que é inviável. <font color=green>Certo.</font>
4. (**1,0 ponto**) Descreva pelo menos um dos quatro níveis de teste constantes da literatura especializada.
**R**: Os quatro níveis de teste incorporados no no planejamento do projeto de testes são os testes de unidade, testes de integração, testes de sistema e testes de aceitação.
No que diz respeito aos testes de unidade, tem como principal objetivo a exploração a menor unidade do projeto, ou seja, testar pequenas funcionalidades isoladamente, sua execução resulta na descoberta de falhas de implementação e lógica nesses pequenos módulos. Atualmente, o teste de unidade é uma boa prática até para os desenvolvedores que devem testar isoladamente métodos e pequenos trechos de código. Para depois juntar os fluxos em testes de integração. <font color=green>Certo.</font>
5. (**1.0 ponto**) Descreva qual o propósito do critério de teste funcional Particionamento por Classes de Equivalência.
**R**: No teste funcional por particionamento em classes de equivalência, propõe a divisão do domínio de entrada em um conjunto especificado de classes de equivalência e a partir dessas classes de equivalência que os casos de teste são especificados, seu principal objetivo é diminuir o número de casos de teste, criando apenas um caso para uma classe de equivalência, pois baseado no princípio das classes de equivalência, todos os elementos de uma classe devem se comportar de maneira equivalente. Também é possível considerar o domínio de saídas para a especificação das classes de equivalência. <font color=green>Certo.</font>
6. (**1.00 ponto**) Existe algum tipo de hierarquia em relação aos critérios de teste estrutural, todos os nós, todos os arcos e todos os caminhos? Se sim, explique-a, considerando a perspectiva dos níveis de cobertura desejados.
**R**: Em relação aos critérios de teste <font color="red">funcional</font>, todos os nós e todos os caminhos, existem sete níveis de hierarquia, e para todos os nós temos o nível 1 que consiste na cobertura de todos comandos ou seja nós, já o nível 2 consiste na cobertura de todos os arcos/arestas e o nível 7 consiste na cobertura de todos os caminhos, juntos podemos cobrir todos os nós, e estruturas e os caminhos possíveis que determinadas condições podem seguir, validando suas saídas. <font color=orange>Parcialmente correto. Nota 0,8.</font>
7. Considere a especificação, a seguir, de um hipotético programa que objtiva a classificação de um triângulo, a partir dos valores informados para os seus três lados.

   a) Dado um triângulo cujos segmentos medem A, B e C, que são números inteiros positivos na faixa de 0 a 100. Esse triângulo somente existirá se: (A + B < C) ou (A + C < B) ou (B + C < A).
   b) Quanto às medidas dos seus lados o triângulo, poderá ser classicado em:
         • Isósceles = quando possui dois lados com a mesma medida;
         • Escaleno = quando todos os seus lados têm medidas diferentes;
         • Equilátero = quando todos os lados tem a mesma medida;
         • Acutângulo = quando o quadrado de um dos seus lados é menor que a soma do quadrado dois outros dois. (A<sup>2</sup> < B<sup>2</sup> + C<sup>2</sup>).
         • Retângulo: quando o quadrado de um dos seus lados é igual à soma do quadrado dois outros dois. (A<sup>2</sup> = B<sup>2</sup> + C<sup>2</sup>).
         • Obtusângulo: quando o quadrado de um dos seus lados é maior que a soma do quadrado dois outros dois. A<sup>2</sup> > B<sup>2</sup> + C<sup>2</sup>.

7.1 (**2.0 pontos**) Definir uma tabela de decisão para o teste tanto da existência do triângulo, quanto para a definição do seu tipo. Consulte exemplo de tabela de decisão na tarefa 005.
Tabela de Decisão

![](https://i.imgur.com/3eYm9Y6.png)

<font color=green>Certo.</font>

7.2 (**2.0 pontos**) Criar os conjunto de casos de teste necessários para a cobertura das combinações constantes da tabela de decisão, seguindo o seguinte padrão:
Casos de Teste

| CT  | Lado A | Lado B | Lado C | Resultado |
| --- | ------ | ------ | ------ | --------- |
| CT1 |10|15|8 |    Não é um triangulo       |
| CT2 |10|10|12|    Isósceles       |
| CT3 |3 |5 |4 |    Escaleno        |
| CT4 |10|10|10|    Equilátero      |

<font color=orange>Parcialmente correto. CT01 Falhou. Nota 1,5.</font>
INSTRUÇÕES:
1. Tipo: Prova individual;
2. Local de Entrega: Plataforma Turing
3. Forma de Entrega: Entregar este arquivo, editado com suas respostas, no formato .md, nominado da seguinte forma: ts2021-2_prova-p1_mat.md, onde mat deverá ser substituído pelo número da sua matrícula.
4. **Entrega diferente da especificada não será avaliada.**
5. Data da Entrega: 22/02/2022, as 23h59min.
6. Critério de Aceitação: arquivo entregue, conforme solicitado.


#### Observação

Referente ao enunciado da questão 7.1 as operações estão com os sinais invertidos (A + B < C) ou (A + C < B) ou (B + C < A), sendo desconsiderado. Portanto a regra passou a ser (A + B > C) ou (A + C > B) ou (B + C > A).
