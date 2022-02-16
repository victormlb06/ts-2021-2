## Tarefa 006 - 15/02/2022 - Grafo de Fluxo de Controle

1. Considere o fragmento de código implementado na Linguagem de Programação Java.

~~~java

public class Avaliacao {


1    public String avalia(double nota1, double nota2, int faltas, int cargaHoraria) throws ValoresInvalidosException{
2        String result;
3        double percentualFaltas = (faltas*100/cargaHoraria);
4        double media = (nota1 + nota2)/2;
5        if((nota1 < 0.0 || nota1 > 10) || (nota2 < 0.0 || nota2 > 10) || (faltas < 0 || faltas > cargaHoraria) || cargaHoraria < 0){
6            throw new ValoresInvalidosException();//result = "Valores Inválidos.";
7        }else if(percentualFaltas > 25.0){
8            result = "Reprovado por Falta.";
9        }else if(media < 3.0){
10            result = "Reprovado por Média.";
11        }else if(media >= 3.0 && media < 6.0){
12            result = "Prova Extra.";
13        }else{
14            result = "Aprovado.";
15        }
16        return result;
17    }
18 }
~~~

2. Pede-se:
   1. Desenhar o **Grafo do Fluxo de Controle**. Pode-se anexar a imagem, aqui neste arquivo.
   2. Calcular a complexidade ciclomática do código. Exemplo de coo calcular pode ser obtido no [link](https://www.treinaweb.com.br/blog/complexidade-ciclomatica-analise-estatica-e-refatoracao)
   3. Definir quantos caminhos de execução existem;
   4. Definir os casos de teste necessários para se percorrer todos estes caminhos. Cada caso de teste deve ter o valor correspondente para cada variável de entrada e o valor esperado.

## Resultados obtidos

1. A imagem do grafo do Fluxo de Controle abaixo foi gerada pelo plugin CFG Generator:
  ![](https://i.imgur.com/8vvT5b2.png)

2. Sobre a questão da complexidade, pode-se dizer que há várias maneiras de se calcular tal valor. Nesse sentido, será escolhida a V(G) = E – N + 2 - onde E é o número de arestas (setas) e N é o número de nós do grafo G. Nesse sentido, o valor da complexidade é 5.

    ![](https://i.imgur.com/ubHpwlO.png)


Uma das referências que se tem é o trabalho de McCabe, o qual fornece alguns valores de parâmetro:

|Complexidade|	Avaliação|
|:-|:-|
1-10|	Método simples. Baixo risco.
11-20|	Método razoavelmente complexo. Moderado risco.
21-50|	Método muito complexo. Elevado risco.
51-N	|Método de altíssimo risco e bastante instável.

Ao observar a tabela, verifica-se que se trata de um método simples.Mas assim como dito acima, são valores de referência, logo pode ocorrer melhoras ou refatorações se necessário.

3. Sobre os caminhos, segue a imagem demonstrando-os:

![](https://i.imgur.com/iZm2Amd.png)

Segue a tabela dos percursos de cada caminho:

Caminho| Percurso|
:-|:-|
C01|ABCDFM|
C02|ABCDEHM|
C03|ABCDEGJM|
C04|ABCDEGILM|
C05|ABCDEGIK|

4. Sobre os casos de teste:

CT|	Valor de entrada (nota1,nota2,faltas,cargaHoraria)|	Resultado Esperado|
|:-|:-|:-|
|CT01|	-2;10;30;100	|Valores inválidos|
|CT02|	10;-2;30;100	|Valores inválidos|
|CT03|	10;10;-3;100	|Valores inválidos|
|CT04|	10;10;-3;100	|Valores inválidos|
|CT05|	10;10;0;-2	|Valores inválidos|
|CT06|	10;10;200;100	|Valores inválidos|
|CT07|	11;10;0;100	|Valores inválidos|
|CT08|	10;11;20;100	|Valores inválidos|
|CT09|	10;8;30;100	|Reprovado por falta|
|CT10|	1;2;20;100	|Reprovado por média|
|CT11|	4;4;20;100	|Prova extra|
|CT12|	10;10;0;100	|Aprovado|