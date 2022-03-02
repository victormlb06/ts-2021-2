# ts2021-2_prova-p1_201800230

<div align=center)>

![](https://i.imgur.com/emRCfbQ.png)


</div>


#### <p style="text-align: center;">Universidade Federal de Goiás</p>
#### <p style="text-align: center;">Instituto de Informática</p>
#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P1 - 16/02/2022</p>

Matrícula: 201800230
Nome: Victor Melo de Lucas Brandão

<p><font color=green>Nota: 9,8.</font></p>

1. Quanto ao objetivo do Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Qual o objetivo primário da atividade de teste de software?

   R: Em face do objetivo primário de teste de software, pode-se dizer que seria revelar a presença de defeitos. <font color=green>Certo.</font>

   2. (**0,5 ponto**) O que acontece, quando não se atinge este objetivo primário?

    R: Sobre a possibilidade do teste não revelar a presença de defeitos, pode-se dizer que, possivelmente, os testes realizados não foram suficientes ou não conseguiram cobrir alguns aspectos que podem estar defeituosos. Logo, poderá descobrir possiveis defeitos no software, sistema ou componente no futuro. <font color=orange>Parcialmente correto. Nota 0,3.</font>


2. (**1,0 ponto**) Explique o que é o teste exaustivo e porque sua execução não é possível.

   R: Em análise ao teste exaustivo, pode-se dizer que será o processo em que serão testados todas as possibilidades das funções de um sistema ou componente. Sendo assim, será feita uma análise especifíca de cada uma das possibilidades do objeto de teste, portanto torna-se impraticável visto que há um grande número de possibilidades. Ademais, em tese, haverá problemas de falta quanto a recursos humanos e computacionais para esse tipo de teste. <font color=green>Certo.</font>

3. (**1,0 ponto**) Cite pelo menos duas limitações da Técnica de Teste Funcional e duas da Técnica de Teste Estrutural.

   R: Em relação as limitações da Técnica de Teste funcional, pode-se citar que é muito dependente de uma boa especificação de requisitos - logo, não há uma garantia da boa execução dessa tarefa - e pode não ser possível garantir que partes essenciais ou critícas do software sejam executadas. Quanto as limitações da técnica de teste estrutural, deve-se citar que um módulo pode executar diversos casos de teste e falhar em alguns outros e defeitos podem existir mesmo com fluxo de controle correto.
<font color=green>Certo.</font>
4. (**1,0 ponto**) Descreva pelo menos um dos quatro níveis de teste constantes da literatura especializada.

   R: Sobre os níveis de teste constantes, pode-se dizer que o nível de teste de integração tem como objetivo provocar falhas associadas as interfaces entre os módulos, sendo esses integrados para construir a estrtura do software que foi estabelecida na fase de projeto. <font color=green>Certo.</font>

5. (**1.0 ponto**) Descreva qual o propósito do critério de teste funcional Particionamento por Classes de Equivlência.

   R: Em relação ao propósito do teste fucional particionamento por classes de equivalência, pode-se dizer eles devem minimizar o número de casos de teste, logo, se seleciona apenas um caso de teste de cada classe visto que deve haver uma equivalência no comportamento de elementos de uma mesma classe. <font color=green>Certo.</font>

6. (**1.00 ponto**) Existe algum tipo de hierarquia em relação aos critérios de teste estrutural, todos os nós, todos os arcos e todos os caminhos? Se sim, explique-a, considerando a perspectiva dos níveis de cobertura desejados.

   R: Em relação a hierarquia aos critérios de teste estrutural de todos os nós, todos os arcos e todos os caminhos, deve-se dizer que há sim uma hierarquia a qual é o nível 1,2 e 7. Quanto ao ponto de vista do primeiro, o qual compreende a cobertura de todos os nós, quanto ao segundo abrange 100% de cobertura de decisões onde cada comando assume valores TRUE e FALSE. Por fim, o nível 7 onde há cobertura de 100% dos caminhos, onde em casos de poucos loops pode acontecer de existir casos de testes suficientes para cobri-los, caso contrário seria impossível compreender todos. <font color=green>Certo.</font>

7. Considere a especificação, a seguir, de um hipotético programa que objtiva a classificação de um triângulo, a partir dos valores informados para os seus três lados.

   a) Dado um triângulo cujos segmentos medem A, B e C, que são números inteiros positivos na faixa de 0 a 100. Esse triângulo somente existirá se: (A + B > C) ou (A + C > B) ou (B + C > A).
   b) Quanto às medidas dos seus lados o triângulo, poderá ser classicado em:
         • Isósceles = quando possui dois lados com a mesma medida;
         • Escaleno = quando todos os seus lados têm medidas diferentes;
         • Equilátero = quando todos os lados tem a mesma medida;
         • Acutângulo = quando o quadrado de um dos seus lados é menor que a soma do quadrado dois outros dois. (A<sup>2</sup> < B<sup>2</sup> + C<sup>2</sup>).
         • Retângulo: quando o quadrado de um dos seus lados é igual à soma do quadrado dois outros dois. (A<sup>2</sup> = B<sup>2</sup> + C<sup>2</sup>).
         • Obtusângulo: quando o quadrado de um dos seus lados é maior que a soma do quadrado dois outros dois. A<sup>2</sup> > B<sup>2</sup> + C<sup>2</sup>.

OBS: Foram trocado os sinais os quais indicam a existência dos triângulos visto que estavam com sinal invertidos. Ademais, foi desconsiderado da atividade os triângulos retângulos, obtusângulo e acutângulo.

7.1 (**2.0 pontos**) Definir uma tabela de decisão para o teste tanto da existência do triângulo, quanto para a definição do seu tipo. Consulte exemplo de tabela de decisão na tarefa 005.

|Causa/Efeito|Regra|R1|R2|R3|R4|R5|R6|R7|R8|R9|
|:-|:-|:-|:-|:-|:-|:-|:-|:-|:-|:-|
|Causa| A+B>C ou A+C>B ou B+C>A|V|V|V|V|V|V|V|V|F|
|Causa| A=B|V|V|V|V|F|F|F|F|F|
|Causa| A=C|V|V|F|F|V|V|F|F|F|
|Causa| B=C|V|F|V|F|V|F|V|F|F|
||||||||||
|Efeito|Triângulo Equilátero|X|||||||||
|Efeito|Triângulo Escaleno||||||||X||
|Efeito|Triângulo Isósceles||||X||X|X|||
|Efeito|Não é triângulo|||||||||X|
|Efeito|Impossível||X|X||X|||||

<font color=green>Certo.</font>

7.2 (**2.0 pontos**) Criar os conjunto de casos de teste necessários para a cobertura das combinações constantes da tabela de decisão, seguindo o seguinte padrão:
|CT|Lado A|Lado B|Lado C|Resultado|
|---|---|---|---|---|
| CT1  | 25  | 25  | 25  | Triângulo Equilátero  |
| CT2  | 14  | 15  | 17  |  Triângulo Escaleno |
| CT3  | 20  | 20  | 15  |  Triângulo Isósceles |
| CT4  | 20  | 15 | 5  | Não é triângulo  |

<font color=green>Certo.</font>
