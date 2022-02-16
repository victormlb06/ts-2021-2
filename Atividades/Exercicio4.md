Nome: Victor Melo de Lucas Brandão Matrícula: 201800230

Conjunto de classes de equivalência

|ID |Descrição| V/I|
|:-|:-|:-|
|CE01| cargahorararia<0| I|
CE02| nota1<0| I| 
CE03| nota2<0| I| 
CE04| faltas<0| I| 
CE05| nota1>100| I|
CE06| nota2>100| I|
CE07| 0>=nota1<=100|V|
CE08| 0>=nota2<=100| V|
CE09| faltas>=0 |V|
CE10| cargahoraria>=0| V|

|CT| Valor de entrada (nota1,nota2,faltas,cargaHoraria)| Resultado Esperado |Classe de equivalência|
|:-|:-|:-|:-|
CT01| 100;100;0;100| Aprovado |CE07,CE08,CE09,CE10|
CT02| 95;80;10;100| Aprovado |CE07,CE08,CE09,CE10| 
CT03| -100;60;0;100| Nota1 inválida|CE02;CE08;CE09;CE10| 
CT04| 100;-60;5;100| Nota2 inválida| CE03;CE07;CE09;CE10 |
CT05 |120;60;20;100 |Nota1 inválida |CE05;CE08;CE09;CE10 |
CT06 |100;170;10;100| Nota2 inválida| CE06;CE07;CE09;CE10|
CT07| 20;30;0;100| Recuperação| CE07,CE08,CE09,CE10| CT08 |45;10;10;100 |Recuperação| CE07,CE08,CE09,CE10|
CT09| 100;100;-2;100| Falta inválida| CE04;CE07;CE08;CE10 |
CT10| 100;100;0;-1| Carga Horária inválida| CE01;CE07;C08;CE09| 
CT11| 100;80;25;100| Aprovado| CE07,CE08,CE09,CE10 |
CT12| 100;100;30;100 |Reprovado por falta| CE07,CE08,CE09,CE10|
CT13| 60;60;25;100| Aprovado| CE07,CE08,CE09,CE10|
CT14| 50;50;0;100| Recuparação| CE07,CE08,CE09,CE10|
CT15| 80;70;0;100 |Aprovado| CE07,CE08,CE09,CE10| 
CT16 |0;0;0;100 |Reprovado |CE07,CE08,CE09,CE10|
CT17| 10;30;0;100| Reprovado| CE07,CE08,CE09,CE10| 
CT18| 40;20;20;100| Reprovado| CE07,CE08,CE09,CE10| 
CT19| 100;90;-1;100 |Falta inválida| CE04;CE07;CE08;CE10| 
CT20| 80;80;10;100 |Aprovado| CE07,CE08,CE09,CE10|