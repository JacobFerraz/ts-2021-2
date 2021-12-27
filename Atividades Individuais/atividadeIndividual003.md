## Tarefa 003 - 21/12/2021 - Defini��o de Classes de Equival�ncia.

**DEFINI��O**:
1. Definir um conjunto de classes de Equival�ncia e um conjunto de casos de testes derivados, para testar a seguinte fun��o de avalia��o universit�ria.
2. A fun��o avalicao, recebe como par�mtros os seguintes dados:
   2.1. **nota1** (num�rico de ponto flutuante com duas casas decimais);
   2.2. **nota2**  (num�rico de ponto flutuante com duas casas decimais);
   2.3. **cargaHoraria** (num�rico inteiro, positivo);
   2.4. **faltas** (num�rico inteiro, positivo).
3. A forma de calcular a avalia��o � a seguinte:
  3.1. Se a quantidade de faltas for superior a 25% da carga hor�ria, o aluno estar� reprovado por falta. Neste caso a fun��o retorna a seguinte mensagem "Reprovado por Falta";
  3.2. Estando o aluno reprovado por falta, n�o haver� a necessidade de se avaliar as notas;
  3.2. Se a m�dia entre nota1 e nota2 for menor que 3.0, o aluno estar� reprovado por m�dia.  Neste caso a fun��o retorna a seguinte mensagem "Reprovado por M�dia";
  3.3. Se a m�dia entre nota1 e nota2 for >= 3.0 e < 6.0, o aluno estar� em recupera��o.  Neste caso a fun��o retorna a seguinte mensagem "Recupera��o";
  3.4 Em qualquer outra situa��o o aluno estar�  aprovado. Ent�o a fun��o retornar� a mensagem: "Aprovado".
4. O Conjunto de classes de Equival�ncia dever� ser definido seguindo o seguinte padr�o:

|id|descri��o|V/I|
|--|--|--|
|CE01|nota1 < 0|I|

Onde:
**CE** = Classe de Equival�ncia, seguido de um n�mero sequencial;
**Descri��o** = define um cen�rio de teste;
**V/I** = V�lida ou Inv�lida.

5. O Conjunto de casos de testes derivado das classes de Equival�ncia deve seguir o seguinte padr�o:

|CT|Valor de Entrada|Resultado Esperado|Classe Equival�ncia|
|--|--|--|--|
|CT01|-2|Valor Inv�lido|CE1|

Onde:
**CT** = Caso de Teste, seguido de um valor sequencial;
**Valor de entrada** � o valor informado para a vari�vel;
**Resultado esperado** � o resultado que se espera da execu��o da fun��o;
**Classe de Equival�ncia** � a identifica��o de qual classe de equival�ncia est� sendo exercitada pelo caso de teste.

INSTRU��ES:
1. Tipo: Esta tarefa � individual;
2. Como responder: Pode-se editar este arquivo, complementando as tabelas de defini��es de classes de equival�ncia e dos casos de teste.
3. Local de Entrega: A entrega dever� seu reposit�rio pessoal, utilizado para a manuten��o dos artefatos de trabalho d disciplina (ts-2021-2);
4. Data da Entrega: Esta tarefa deve estar dispon�vel para avalia��o at� o dia 28/12/2021 �s 23h59min.
5. Crit�rio de Aceita��o: tarefa entregue conforme especificado e na data definida.
6. Caso necessite de suporte, pode encaminhar mensagem para o professor.

**Respostas**

Classes de Equival�ncia
|id|descri��o|V/I|
|--|--|--|
|CE01|Tamanho das casas decimais > 2 da vari�vel nota1|I|
|CE02|Tamanho das casas decimais > 2 da vari�vel nota2|I|
|CE03|nota1 < 0|I|
|CE04|nota1 > 10|I |
|CE05|nota1 > 0 e nota1<10|V|
|CE06|nota2 < 0|I|
|CE07|nota2 > 10|I|
|CE08|nota2 > 0 e nota2<10|V|
|CE09|cargaHoraria < 0|I|
|CE10|cargaHoraria > 0|V|
|CE11|Tamanho das casas decimais > 0 da vari�vel cargaHoraria |I|
|CE12|faltas < 0|I|
|CE13|faltas > 0|V|
|CE14|faltas contem caractere alfab�ticos |I|
|CE15|faltas possui apenas caracteres num�ricos |V|
|CE16|nota1 contem caractere alfab�ticos |I|
|CE17|nota1 possui apenas caracteres num�ricos |V|
|CE18|nota2 contem caractere alfab�ticos |I|
|CE19|nota2 possui apenas caracteres num�ricos |V|
|CE20|cargaHoraria contem caractere alfab�ticos |I|
|CE21|cargaHoraria possui apenas caracteres num�ricos |V|

Conjunto de casos de testes
|CT|Valor de Entrada|Resultado Esperado|Classe Equival�ncia|
|--|--|--|--|
|CT01|nota1=7.00,nota2=7.00,cargaHoraria=100,faltas=50|Reprovado por Falta|CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT02|cargaHoraria=100,faltas=50|Reprovado por Falta|CE10,CE13,CE15,CE21|
|CT03|nota1=2.00,nota2=3.00,cargaHoraria=100,faltas=0|Reprovado por M�dia|CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT04|nota1=5.00,nota2=5.00,cargaHoraria=100,faltas=0|Recupera��o|CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT05|nota1=8.00,nota2=8.00,cargaHoraria=100,faltas=0|Aprovado|CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT06|nota1=8.00,nota2=8.00,cargaHoraria=100,faltas=49|Aprovado|CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT07|nota1=6.00,nota2=6.00,cargaHoraria=100,faltas=49|Aprovado|CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT08|nota1=5.99,nota2=5.99,cargaHoraria=100,faltas=49|Recupera��o|CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT09|nota1=5,nota2=5.99,cargaHoraria=100,faltas=49|nota1 Invalida|CE01,CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT10|nota1=5,nota2=5.00,cargaHoraria=100,faltas=49|nota1 Invalida, nota2 Invalida|CE01,CE02,CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT11|nota1=-1.00,nota2=5.00,cargaHoraria=100,faltas=49|nota1 Invalida|CE01,CE03,CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT12|nota1=11.00,nota2=5.00,cargaHoraria=100,faltas=49|nota1 Invalida|CE01,CE04,CE05,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT13|nota1=5.00,nota2=-1.00,cargaHoraria=100,faltas=49|nota2 Invalida|CE01,CE02,CE03,CE06,CE08,CE10,CE13,CE15,CE17,CE19,CE21|
|CT14|nota1=5.00,nota2=11.00,cargaHoraria=100,faltas=49|nota2 Invalida|CE01,CE02,CE03,CE06,CE07,CE10,CE13,CE15,CE17,CE19,CE21|
