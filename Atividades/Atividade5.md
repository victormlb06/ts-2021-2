## Grafo

![](https://i.imgur.com/t3Xo7jc.png)


## Tabela de Decisão

| CAUSA/EFEITO          | REGRA               |R1|R2|R3|R4|R5|R6|R7|R8|
| ----------------- |:----------------------- |:--|:--|:--|:--|:--|:--|:--|:--|
| CAUSA     | Masculino                        |V|V|V|V|F|F|F|F|
| CAUSA |       Idade>25                  |V|V|F|F|V|V|F|F|
| CAUSA         |  Casado(a)   |V|F|V|F|V|F|V|F|
| EFEITO       | 0% Desconto    | X||||||||
| EFEITO  | 5% Desconto ||X|||X||||||
|EFEITO| 10% Desconto |||X|||X||||
|EFEITO| 15% Desconto ||||X|||X||
|EFEITO| 20% Desconto ||||||||X|

## Caso de Teste

|Caso de Teste | Masculino | Idade>25 | Casado(a) | Valor |
|-|:-|:-|:-|:-|
|CT 1| Verdadeiro |Falso | Falso |R$ 2000,00|
|CT 2| Verdadeiro | Falso | Verdadeiro |R$ 1900,00|
|CT 3| Verdadeiro | Verdadeiro | Falso |R$ 1800,00|
|CT 4| Verdadeiro | Verdadeiro | Verdadeiro |R$ 1700,00|
|CT 5| Falso | Falso| Falso |R$ 1900,00|
|CT 6| Falso | Falso | Verdadeiro |R$ 1800,00|
|CT 7| Falso | Verdadeiro | Falso |R$ 1700,00|
|CT 8| Falso | Verdadeiro | Verdadeiro |R$ 1600,00|