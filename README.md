# Algoritmo-Genetico-Fuzzy

# **Lógica Fuzzy**
> A Lógica Fuzzy (Nebulosa ou Difusa), comumente tratada como uma extensão da lógica booleana, é uma lógica multivalorada capaz de capturar informações vagas, em geral descritas em uma linguagem natural, e convertê-las para um formato numérico.
* Um valor lógico difuso, conhecido por grau de pertinência, é um valor qualquer no intervalo [0, 1].
  * Determina o grau em que um determinado elemento pertence a um conjunto, permitindo uma transição gradual da falsidade para a verdade.
  * Não existe uma base formal para determinar esse valor que é escolhido experimentalmente. 

> As implementações da lógica difusa permitem que estados não precisos possam ser tratados por dispositivos de controle.
 * Desse modo, é possível avaliar conceitos não quantificáveis.
 * Casos práticos: 
  * Avaliar a temperatura (quente, morno, frio, ...)
  * Sentimento de felicidade (radiante, feliz, apático,
triste, ...)

# **Sistema Fuzzy**
> Sistemas são desenvolvidos para resolver problemas. Assim, precisamos do problema que pretendemos resolver através de um Sistema Fuzzy, o qual pode ser visto abaixo.

>**Problema:** 
Uma empresa de alimentos deseja saber a validade real de um de seus produtos em função da temperatura e umidade relativa do ambiente de armazenamento. A validade máxima desse produto é de 42 dias se armazenado a baixa temperatura em ambiente seco. 

> O projeto do Sistema Fuzzy será organizado conforme as três etapas do raciocínio fuzzy:
1.   Fuzzificação
2.   Inferência Fuzzy
3.   Defuzzificação

# **Fuzzificação**
> Etapa na qual as variáveis linguísticas são definidas de forma subjetiva, bem como as funções membro (funções de pertinência)

> Engloba:
* Análise do Problema
* Definição das Variáveis
* Definição das Funções de pertinência
* Criação das Regiões

> Na definição das funções de pertinência para cada variável, diversos tipos de espaço podem ser gerados:
* Triangular, Trapezoidal, Gaussiana, ...

> Assim, segundo o **problema** apresentado, estamos desenvolvendo um Sistema Fuzzy que modela a validade do produto com base na Temperatura (T) e Umidade Relativa (UR) do depósito. A T é um valor entre 0 e 30 ºC, a UR entre 0 e 100 % e Validade de 0 a 42 dias.
* Variáveis de Entrada:
  * Temperatura:
    * Universo (intervalo de valores): [0, 30]
    * Conjuntos Fuzzy/Funções de Pertinência: fria, amena, quente
  * Umidade Relativa:
    * Universo (intervalo de valores): [0, 100]
    * Conjuntos Fuzzy/Funções de Pertinência: baixa, média, alta
* Variáveis de Saída:
  * Validade:
    * Universo (intervalo de valores): [0, 42]
    * Conjuntos Fuzzy/Funções de Pertinência: curta, aceitável, longa

# **Inferência Fuzzy**
> Etapa na qual as proposições (regras) são definidas e depois são examinadas
paralelamente.

> Engloba:
* Definição das proposições
* Análise das regras
* Criação da região resultante

> Definição das Proposições para o Sistema Fuzzy de controle da validade.
* Base de Conhecimento/Regras
  * **SE** a temperatura é fria **E** umidade é baixa **ENTÃO** a validade é longa
  * **SE** a temperatura é quente **OU** umidade é alta **ENTÃO** a validade é curta
  * **SE** a umidade é média **ENTÃO** a validade é aceitável 
# **Defuzzificação**
> Etapa na qual as regiões resultantes são convertidas em valores para a variável de saída do sistema.


