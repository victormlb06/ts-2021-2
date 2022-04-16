#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P2 - 12/04/2022</p>

Matrícula: 201800230

Nome: Victor Melo de Lucas Brandão

<font color="red">Nota 7,07</font>


1. Quanto ao Processo de Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Defina os seguintes conceitos Processo de Teste de Software, Projeto de Teste de Software e Plano de Teste de Sofware.

    R: Em análise aos conceitos de citados no enunciado, pode-se dizer que o Processo de Teste de Software trata-se de uma estruturação de etapas, atividades, artefatos, pápeis e responsabilidades do teste os quais irão permitir que a organização tenha total controle do ciclo de teste, minimize os riscos e agregue valor. Já quanto ao projeto de teste de software, deve-se dizer que seria um documento o qual especifica os detalhes de uma abordagem de teste para um requisito do software ou combinação deles e assim consegue identificar casos de teste associados. Em face do plano de teste de software, deve-se dizer que seria um documento ou mapa no qual há uma definição do escopo e objetivos. Ademais, pode-se acrescentar nele os requisitos, estratégias e recursos a serem empregados nas atividades de testes de software. <font color="red">Nota 0,5</font>

   3. (**0,5 ponto**) Descreva o relacionamento existente entre estes conceitos.

    R: Sobre a relação dos conceitos descritos na questão anterior, pode-se dizer que o processo, como um documento que define as atividades, irá ter como algumas delas, o plano de teste de software e o projeto de teste. O plano por si consegue definir objetivos da atividade de testes os quais são explorados no projeto de teste, ou seja, ele irá auxiliar na atividade de teste do projeto. Enquanto o projeto de teste irá identificar os casos de testes associados com uma base no próprio plano de teste como nos objetivos gerais do processo. <font color="red">Nota 0,5</font>

2. (**1,0 pontos**) Descreva as vantagens para a equipe de desenvolvimento ao se adotar um processo de teste ágil.

    R: Em relação as vantagens para a equipe de desenvolvimento ao adotar um teste ágil, pode-se dizer que oferece uma melhor qualidade do processo e na qualidade do produto. Quanto aos bugs, eles são identifcados, relatados e corrigidos de maneira mais rápida e em um curto espaço de tempo, além do foco na prevenção. A gestã de defeitos passa a ser mais dinâmica e é executada diretamente pelo desenvolvedor. Por fim, a tendência é que as entregas sejam feitas mais rápidas e em curtas interações. <font color="red">Nota 1,0</font>

4. (**1,0 ponto**) Cite pelo menos três características do Teste Exploratório.

    R: Em análise ao teste exploratório, pode-se dizer que são exemplos de teste em que os profissionais (testadores) podem interagir com a aplicação e usar as informações para tomar certas decisões. Ademais, os resultados de teste, casos de teste e documentação de teste são geradas a medida que os testes são realizados os quais podem ser coletados por ferramentas de captura de tela e registros de tecla. Uma última característica, a qual pode se caracterizar também como um defeito, é a necessidade do testador ter conhecimento da aplicação que está testando para ser efetivo onde irá aplicar os testes e ainda demorar uma quantidade significativa de tempo para exercer tais atividades. <font color="red">Nota 1,0</font>

6. Considere os arquivos .java (Banco.java, Agencia.java, Conta.java e BankValidator.java). Nos próprios arquivos .java estão definidas as regras para cadastramento de cada um deles (Banco, Agencia e Conta). Desta forma, pede-se:
   4.1 (**2.0 Pontos**) Definir os cenários de teste suficientes para testar o cadastro e movimentações financeiras envolvendo bancos, agências e contas, conforme especificado. Para cada cenário definir os critérios de teste adequados à definição dos seus casos de teste.
    R:
    Agência:
        *  CE01 - Número da Agência com 4 digitos - Correto;
        *  CE02 - Número da Agência com 2 digitos - Errado;
        *  CE03 - Número da Agência com 6 digitos - Errado;
        *  CE04 - Nome da Agência com 4 caracteres - Errado;
        *  CE05 - Nome da Agência com 7 caracteres - Correto;
        *  CE06 - Nome da Agência com 101 caracteres - Errado;
        *  CE07 - Nome da cidade da Agência com 4 caracteres - Errado;
        *  CE08 - Nome da cidade da Agência com 7 caracteres - Correto;
        *  CE09 - Nome da cidade da Agência com 101 caracteres - Errado;

    Banco:
        *  CE10 - Nome da cidade do Banco com 4 caracteres - Errado;
        *  CE11 -Nome da cidade do Banco com 7 caracteres - Correto;
        *  CE12 - Nome da cidade do Banco com 101 caracteres - Errado;
        *  CE13 -Numero do Banco com 4 digitos - Errado;
        *  CE14 - Numero do Banco com 2 digitos - Errado;
        *  CE15 - Numero do Banco com 3 digitos - Correto;
        *  CE16 - Numero do Banco com valores negativos - Errado;
        *  CE17 - Nome da cidade do Banco com números - Errado;
        *  CE18 - Numero do Banco com 3 digitos decimais - Errado;

    Conta:
        *  CE19 - Valida tipo de conta investimento - Errado
        *  CE20 - Valida tipo de conta Poupança - Correto
        *  CE21 - Valida tipo de conta Corrente - Correto
        *  CE22 - Valida saque com saldo negativo - Errado
        *  CE23 - Valida saque com saldo positivo - Correto
        *  CE24 - Valida transferência com saldo negativo - Errado;
        *  CE25 - Valida transferência com saldo positivo - Correto;
        *  CE26 - Valida depositar valor negativo - Errado;
        *  CE27 - Valida depositar valor positivo - Correto;
        *  CE28 - Valida creditar rendimentos com valor positivo - Correto;
        *  CE29 - Valida creditar rendimentos com valor negativo - Errado;
        *  CE30 - Valida debitar juros do cheque especial com valor positivo - Correto;
        *  CE31 - Valida debitar juros do cheque especial com valor negativo - Errado;

      <font color="red">Nota 1,5</font>

   3. (2.0) Definir os casos de teste suficientes para a cobertura do teste de cada um dos cenários definidos. Documentar os casos de teste no seguinte padrão:


   | CT| CE| Valores de Entrada| Resultado esperado |
   | - | --  |------------------ | ------------------ |
   | CT01 | CE01 | 123                    | True               |
   | CT02 | CE02 | 12                     | False              |
   | CT03 | CE03 | 123456                 | False              |
   | CT04 | CE04 | abcd                   | False              |
   | CT05 | CE05 | Goiania                | True               |
   | CT06 | CE06 | (valor 100 caracteres) | False              |
   | CT07 | CE07 | abcd                   | False              |
   | CT08 | CE08 | Goiania                | True               |
   | CT09 | CE09 | (valor 100 caracteres) | False              |
   | CT10 | CE10 | abcd                   | False              |
   | CT11 | CE11 | Goiania                | True               |
   | CT12 | CE12 | (valor 100 caracteres) | False              |
   | CT13 | CE13 | 1234                   | False              |
   | CT14 | CE14 | 12                     | False              |
   | CT15 | CE15 | 123                    | True               |
   | CT16 | CE16 | -123                   | False              |
   | CT17 | CE17 | 123456                 | False              |
   | CT18 | CE18 | 0.123124               | False              |
   | CT19 | CE19 | Investimento           | False              |
   | CT20 | CE20 | Poupança               | True               |
   | CT21 | CE21 | Corrente               | True               |
   | CT22 | CE22 | 123,-12000             | False              |
   | CT23 | CE23 | 123, 12000             | True               |
   | CT24 | CE24 | 123,-12000             | False              |
   | CT25 | CE25 | 123,12000              | True               |
   | CT26 | CE26 | 123,-12000             | False              |
   | CT27 | CE27 | 123,12000              | True               |
   | CT28 | CE28 | 123,12000              | True               |
   | CT29 | CE29 | 123,-12000             | False              |
   | CT30 | CE30 | 123,12000              | True               |

   <font color="red">Nota 1,5</font>

   3. (3.0 Pontos) Implementar (na linguagem de programação java) as classes para o teste da criação dos objetos e das movimentações financeiras envolvendo bancos e agências e contas.

   <font color="red">Nota 1,07</font>

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
