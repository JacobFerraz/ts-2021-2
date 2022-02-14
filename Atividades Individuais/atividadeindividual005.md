## Tarefa 005 - 08/02/2022 - Grafo de Causa e Efeito / Tabela de Decisão.

1.Considere o seguinte cenário: Uma corretora de seguros concede desconto sobre o prêmio anual de seguro de automóvel, aos seus segurados conforme as regras a seguir:
|Sexo|Idade (anos)|Estado Civil|Desconto (%)|
|---|---|---|---|
|Masculino|< 25|Solteiro|0|
|Masculino|< 25|Casado|5|
|Masculino|> 25|Solteiro|10|
|Masculino|> 25|Casado|15|
|Feminino|< 25|Solteira|5|
|Feminino|< 25|Casada|10|
|Feminino|> 25|Solteira|15|
|Feminino|> 25|Casada|20|

2. Solicita-se:
   1. Geração do grafo de causa e efeito para representar este cenário.
      1. Anexar a este arquivo a imagem do grafo.
   2. Geração da tabela de decisão para representar o cenário.
      1. Editar este arquivo e adicionar a tabela de decisão.
   3. Geração do conjunto de casos de teste suficientes para cobrir todos os cenários, constantes do grafo e da tabela de decisão.
      1. Editar este arquivo e adicionar a tabela com os casos de teste, conforme exemplos disponibilizados em tarefas anteriores.
   4. Em relação aos casos de teste, considere o valor do seguro de R$ 2.000,00 (Dois mil reais). Desta forma, o valor esperado, do resultado do caso de teste, deve ser o valor líquido a ser pago. Ou seja, o prêmio deduzido do valor correspondente ao percentual do desconto obtido pelo cliente.
INSTRUÇÕES:
1. Tipo: Tarefa Individual;
2. Local de Entrega: Repositório pessoal, no github. O arquivo a ser entregue é este mesmo, editado com a inclusão dos dados solicitados.
3. Data da Entrega: 14/02/2022, as 23h59min.
4. Critério de Aceitação: Arquivo entregue com os dados solicitados.

**Respostas**

1. Grafo de causa efeito

![](https://i.imgur.com/KwchjEx.png)

2. Tabela de decisão

||Regra 1|Regra 2|Regra 3|Regra 4| Regra 5| Regra 6|Regra 7| Regra 8
|---|---|---|---|---|---|---|---|---|
|Condições|||||
|Masculino?|SIM|SIM|SIM|SIM|NÃO|NÃO|NÃO|NÃO
|Casado?|SIM|SIM|NÃO|NÃO|SIM|SIM|NÃO|NÃO
|Idade maior que 25?|SIM|NÃO|SIM|NÃO|SIM|NÃO|SIM|NÃO

3. Casos de Teste

|CT|Valor de Entrada|Resultado Esperado
|--|--|--
|CT01|Masculino, 26, Solteiro |Desconto 10%
|CT02|Masculino, 26, Casado |Desconto 15%
|CT03|Masculino, 24, Solteiro|Sem Desconto
|CT04|Masculino, 24, Casado|Desconto 5%
|CT05|Feminino, 26, Solteiro|Desconto 15%
|CT06|Feminino, 26, Casado|Desconto 20%
|CT07|Feminino, 24, Solteiro|Desconto 5%o
|CT08|Feminino, 24, Casado|Desconto 10%
