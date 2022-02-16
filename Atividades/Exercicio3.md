Nome: Victor Melo de Lucas Brandão
Matrícula: 201800230

Conjunto de classes de equivalência

|ID|	Descrição|	V/I|
|:-|:-|:-|
CE01	|cargahorararia<0|	I
CE02	|nota1<0	|I
CE03	|nota2<0|	I
CE04	|faltas<0|	I
CE05	|nota1>100|	I
CE06	|nota2>100|	I
CE07	|nota1>=0 e nota1<=100|	V
CE08	|nota2>=0 e nota2<=100|	V
CE09	|faltas>=0|	V
CE10	|cargahoraria>=0|	V

CT|	Valor de entrada (nota1,nota2,faltas,cargaHoraria)|	Resultado Esperado	|Classe de equivalência
|:-|:-|:-|:-|
CT01|	10;10;30;100	|Reprovado por Falta|	CE07,CE08,CE09,CE10
CT02|	20:20:0:100|	Reprovado por média|	CE07,CE08, CE09,CE10
CT03|	40;40;0;100	|Recuperação	|CE07,CE08, CE09,CE10
CT04|	100;100;0;100	|Aprovado|	CE07,CE08, CE09,CE10
CT05|	110;100;0;100|	Valor inválido|	CE05,CE08, CE09,CE10
CT06|	100;110;0;100|	Valor inválido|	CE06,CE08, CE09,CE10
CT07|	100;100;-4;100|	Valor inválido|	CE04,CE08, CE09,CE10
CT08|	100;100;0;-9|	Valor inválido	|CE01,CE08, CE09,CE10
CT09|	110;110;0;100	|Valor inválido|	CE05,CE06, CE09,CE10
CT10|	110;100;-4;100|	Valor inválido	|CE05,CE04, CE08,CE10
CT11|	110;100;0;-2	|Valor inválido|	CE01,CE05,CE08, CE09
CT12|	110,110,-2;100|	Valor inválido|	CE05,CE06,CE04,C10
CT13|	110;110;0;-4|	Valor inválido|	CE01,CE05,CE06,CE09
CT14|	110;100;-2;-4|	Valor inválido |CE01,CE04CE05, CE08
CT15|	100;110;-2;-4|	Valor inválido|	CE01,CE04,CE06,CE07
CT16|	-2;-2;-2;-2|	Valor inválido|	CE01,CE02,CE03,CE04
