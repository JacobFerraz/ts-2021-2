## Tarefa 003 - 21/12/2021 - Definição de Classes de Equivalência.

**DEFINIÇÃO**:
1. Definir um conjunto de classes de Equivalência e um conjunto de casos de testes derivados, para testar a seguinte função de avaliação universitária.
2. A função avalicao, recebe como parâmtros os seguintes dados:
   2.1. **nota1** (numérico de ponto flutuante com duas casas decimais);
   2.2. **nota2**  (numérico de ponto flutuante com duas casas decimais);
   2.3. **cargaHoraria** (numérico inteiro, positivo);
   2.4. **faltas** (numérico inteiro, positivo).
3. A forma de calcular a avaliação é a seguinte:
  3.1. Se a quantidade de faltas for superior a 25% da carga horária, o aluno estará reprovado por falta. Neste caso a função retorna a seguinte mensagem "Reprovado por Falta";
  3.2. Estando o aluno reprovado por falta, não haverá a necessidade de se avaliar as notas;
  3.2. Se a média entre nota1 e nota2 for menor que 3.0, o aluno estará reprovado por média.  Neste caso a função retorna a seguinte mensagem "Reprovado por Média";
  3.3. Se a média entre nota1 e nota2 for >= 3.0 e < 6.0, o aluno estará em recuperação.  Neste caso a função retorna a seguinte mensagem "Recuperação";
  3.4 Em qualquer outra situação o aluno estará  aprovado. Então a função retornará a mensagem: "Aprovado".
4. O Conjunto de classes de Equivalência deverá ser definido seguindo o seguinte padrão:

|id|descrição|V/I|
|--|--|--|
|CE01|nota1 < 0|I|

Onde:
**CE** = Classe de Equivalência, seguido de um número sequencial;
**Descrição** = define um cenário de teste;
**V/I** = Válida ou Inválida.

5. O Conjunto de casos de testes derivado das classes de Equivalência deve seguir o seguinte padrão:

|CT|Valor de Entrada|Resultado Esperado|Classe Equivalência|
|--|--|--|--|
|CT01|-2|Valor Inválido|CE1|

Onde:
**CT** = Caso de Teste, seguido de um valor sequencial;
**Valor de entrada** é o valor informado para a variável;
**Resultado esperado** é o resultado que se espera da execução da função;
**Classe de Equivalência** é a identificação de qual classe de equivalência está sendo exercitada pelo caso de teste.

INSTRUÇÕES:
1. Tipo: Esta tarefa é individual;
2. Como responder: Pode-se editar este arquivo, complementando as tabelas de definições de classes de equivalência e dos casos de teste.
3. Local de Entrega: A entrega deverá seu repositório pessoal, utilizado para a manutenção dos artefatos de trabalho d disciplina (ts-2021-2);
4. Data da Entrega: Esta tarefa deve estar disponível para avaliação até o dia 28/12/2021 às 23h59min.
5. Critério de Aceitação: tarefa entregue conforme especificado e na data definida.
6. Caso necessite de suporte, pode encaminhar mensagem para o professor.

**Respostas**

Classes de Equivalência
|id|descrição|V/I|
|--|--|--|
|CE01|Tamanho das casas decimais > 2 da variável nota1|I|
|CE02|Tamanho das casas decimais > 2 da variável nota2|I|
|CE03|nota1 < 0|I|
|CE04|nota1 > 10|I |
|CE05|nota1 > 0 e nota1<10|V|
|CE06|nota2 < 0|I|
|CE07|nota2 > 10|I|
|CE08|nota2 > 0 e nota2<10|V|
|CE09|cargaHoraria < 0|I|
|CE10|cargaHoraria > 0|V|
|CE11|Tamanho das casas decimais > 0 da variável cargaHoraria |I|
|CE12|faltas < 0|I|
|CE13|faltas > 0|V|
|CE14|faltas contem caractere alfabéticos |I|
|CE15|faltas possui apenas caracteres numéricos |V|
|CE16|nota1 contem caractere alfabéticos |I|
|CE17|nota1 possui apenas caracteres numéricos |V|
|CE18|nota2 contem caractere alfabéticos |I|
|CE19|nota2 possui apenas caracteres numéricos |V|
|CE20|cargaHoraria contem caractere alfabéticos |I|
|CE21|cargaHoraria possui apenas caracteres numéricos |V|

Conjunto de casos de testes
|CT|Valor de Entrada|Resultado Esperado|Classe Equivalência|
|--|--|--|--|
|CT01|nota1=7.00,nota2=7.00,cargaHoraria=100,faltas=50|Reprovado por Falta|CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT02|cargaHoraria=100,faltas=50|Reprovado por Falta|CE10,CE13,CE15,CE21|
|CT03|nota1=2.00,nota2=3.00,cargaHoraria=100,faltas=0|Reprovado por Média|CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT04|nota1=5.00,nota2=5.00,cargaHoraria=100,faltas=0|Recuperação|CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT05|nota1=8.00,nota2=8.00,cargaHoraria=100,faltas=0|Aprovado|CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT06|nota1=8.00,nota2=8.00,cargaHoraria=100,faltas=49|Aprovado|CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT07|nota1=6.00,nota2=6.00,cargaHoraria=100,faltas=49|Aprovado|CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT08|nota1=5.99,nota2=5.99,cargaHoraria=100,faltas=49|Recuperação|CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT09|nota1=5,nota2=5.99,cargaHoraria=100,faltas=49|nota1 Invalida|CE01,CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT10|nota1=5,nota2=5.00,cargaHoraria=100,faltas=49|nota1 Invalida, nota2 Invalida|CE01,CE02,CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT11|nota1=-1.00,nota2=5.00,cargaHoraria=100,faltas=49|nota1 Invalida|CE01,CE03,CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT12|nota1=11.00,nota2=5.00,cargaHoraria=100,faltas=49|nota1 Invalida|CE01,CE04,CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT13|nota1=5.00,nota2=-1.00,cargaHoraria=100,faltas=49|nota2 Invalida|CE01,CE02,CE03,CE06,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT14|nota1=5.00,nota2=11.00,cargaHoraria=100,faltas=49|nota2 Invalida|CE01,CE02,CE03,CE06,CE07,CE10,CE13,CE15,CE17,CE19,CE21|
