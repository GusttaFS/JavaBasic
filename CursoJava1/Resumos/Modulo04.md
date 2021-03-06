## Índice
- [Algoritmos](#algoritmo)
- [Escrevendo algoritmos em pseudocódigo](#pencil-escrevendo-algoritmos-em-pseudocódigo)
- [Variáveis](#file_folder-variáveis)
    - [Definição de nome da variável](#definição-de-nome-da-variável)
    - [Tipos de variáveis](#tipos-de-variáveis)
    - [Declaração de variáveis em pseudocódigo](#declaração-de-variáveis-em-pseudocódigo)
    - [Operação de atribuição](#arrow_left-operação-de-atribuição)
- [Comando leia](#inbox_tray-comando-leia)
- [Realizando cálculos](#symbols-realizando-cálculos)
- [Saída de dados](#outbox_tray-saída-de-dados)
- [Primeiro Algoritmo](#bar_chart-Primeiro-algoritmo)

# Introdução à Programação

## Algoritmo


Sequência lógica de passos do programa, que pode ser expressa em qualquer linguagem de programação.
<img src="https://github.com/LeandraOliveiraS/JavaBasic/blob/master/CursoJava1/imagens/4-algoritmo.png?raw=true" width = "60%" height= "50%">

Existem várias formas informais para se escrever rascunhos de códigos, dentre as mais utilizadas encontram-se:

- **Descrição narrativa**: que é uma representação textual simples das instruções do algoritmo.
Esta forma é **pouco** utilizada, pois, as instruções podem ser ambíguas e de difícil representação em uma linguagem de programação.

- **Diagramas de Chapin**: são uma representação gráfica das instruções de um algoritmo de forma *hierárquica e estruturada*. São pouco usados em desenvolvimento de programas, mas bastante representativos.
    <img src="https://arquivo.devmedia.com.br/artigos/Gabriel_Giaretta/Diagramas-Chapin-Fluxogramas/Diagramas-Chapin-Fluxogramas7.jpg" width = "30%" height = "30%" text-align= "middle">

- **Fluxogramas**: também conhecidos como diagrama de blocos, que utilizam figuras geométricas para identificar tipos diferentes de instruções.
São bastante utilizados para representar algoritmos, inclusive em outras áreas além da programação.
    <img src= "https://github.com/LeandraOliveiraS/JavaBasic/blob/master/CursoJava1/imagens/6-fluxograma.png?raw=true" width = "60%" height = "60%">

- **Pseudocódigo**: também conhecido como ***português estruturado*** ou portugol. É uma representação de algoritmos baseada nas regras da linguagem [pascal]().
Esta forma de representação, junto com os fluxogramas, são uma das mais utilizadas para se representar algoritmos em programação.


    ```
    
    Algoritmo "Verifica idade"

    var
    idade: inteiro

    início
        escreva "Informe sua idade"
        leia idade
        se idade < 25 então
            escreva "você é jovem!"
        senão
            escreva "você já não é mais tão jovem assim kk!"
        fim se
    fim
    
    ```

## :pencil: Escrevendo algoritmos em pseudocódigo

Todo algoritmo em pseudocódigo deve ser escrito utilizando uma estrutura básica:

```

Algoritmo "nome do algoritmo"

var
declaração de variáveis

início
    instruções 

fim

```

---


## :file_folder: Variáveis

A memória de um computador pode ser vista como um conjunto de células, onde dados de diversos tipos podem ser armazenados.
Cada uma das células de memória é identificada por um **endereço númerico**.
    Assim, para acessar um determinado dado na memória, seria necessário conhecer a posição inicial deste dado na mémoria e quantos bytes foram usados para armazená-lo.

Para facilitar que os programadores acessem esses dados de forma facilitada, criou-se o conceito de **variável**.

> :warning: Cada variável representa uma ou mais posições de memória onde um determinado dado encontra-se armazenado.


### Definição de nome da variável

Toda variável possui um nome que tem a função de diferencia-la das demais.
Cada linguagem de programação estabelece as suas próprias regras de formação de nomes de variáveis.
    
As **regras** mais adotadas são as seguintes:
- Nome de variável deve necessariamente começar com uma letra ou sublinhado.
- Um nome de variável não deve conter nenhum símbolo especial, exceto o sublinhado.
- Após o primeiro caractere podem ser empregados dígitos numéricos.
- Não pode haver espaços em branco entre os caracteres, para substituí-los use o sublinhado.
- Devem ser evitadas letras com acentuação.

**Exemplos**:

Variável| Corretude
:---:|:---:
salario|:heavy_check_mark:
1ano| :x:
ano1|:heavy_check_mark:
a casa| :x:
sal/hora|:x:
sal_hora|:heavy_check_mark:
_desconto|:heavy_check_mark:


### Tipos de variáveis 

O tamanho de uma variável é definido pelo seu tipo. O tipo de uma variável define quais dados podemos atribuir a ela. Mas quais tipos podemos associar a uma variável?

A maioria das linguagens de programação de alto nível trabalham com cinco tipos de dados básicos, chamados **tipos primitivos**.

Tipo| Definição
:---:| ---
**inteiro**| Todos os números positivos, negativos e o zero.
**real**| Números com parte fracionária.
**lógico**| Valores verdadeiros (*true*) ou falsos (*false*).
**caractere**| Símbolos alfanúmericos, letras, algarismos, sinais de pontuação e qualquer outro símbolo válido.                                                 Devem ser representados entre *aspas simples* (' ').
**literal**| Também chamado de cadeia de caractere ou **string**. Devem ser representados entre ***aspas duplas*** (" ").


### Declaração de variáveis em pseudocódigo

Todas as variáveis utilizadas em algoritmos devem ser **declaradas** antes de serem utilizadas.
Declarar uma variável é dizer, a priori, o nome e o tipo de cada variável utilizada. Isto se faz necessário para que seja
reservado um espaço de memória para as mesmas.
O exemplo abaixo ilustra bem como deve ser realizada esta declaração.

``` var
nome, endereço: literal
idade: inteiro
salario: real
tem_filhos: lógico
```

### :arrow_left: Operação de atribuição

A atribuição de valores a uma variável é realizada da seguinte forma:

``nome da variável <- valor``

> O valor expresso ao lado direito é armazenado na variável informada à esquerda.

Exemplo:

```
numero <- 3
var <- 2 * numero
resultado <- var 
```

## :inbox_tray: Comando leia

O comando leia recebe valores digitados pelo o usuário. Logo após este recebimento, os valores são armazenados nas variáveis.

Enquanto esse valor não for recebido, a execução do `leia` ficará esperando o usuário enviar o dado.

**Sintaxe do comando**:

`leia num1, num2`

## :symbols: Realizando Cálculos

Operador| Símbolo
:---:|:---:
Adição|+
Subtração|-
Multiplicação|*
Divisão|div
Resto da divisão|mod


## :outbox_tray: Saída de Dados
Para realizar saída de dados, utilizando um dispositivo de saída, podemos utilizar o comando `escreva`. Este comando possui a seguinte estrutura básica:

`escreva lista_de_valores`
Este comando irá escrever na tela do dispositivo utilizado pelo usuário a resposta produzida pelo algoritmo.


## :bar_chart: Primeiro algoritmo

Utilizando todas as regras e conhecimentos adquiridos ao longo deste resumo, somos capazes de construir uma infinidade de algoritmos. Sendo assim, vamos treinar!

**Exemplo**:

```
"Algoritmo "Cálculo da média de um aluno"
    var 
    nota1, nota2, nota3, nota4, media: real

início

    leia nota1, nota2, nota3, nota4
    media <- (nota1 + nota2 + nota3 + nota4)/4
    escreva media
fim
```

> :warning: É importante notar que o cálculo da média está sendo realizado utilizando parênteses. 

Pois, na programação são utilizadas as **mesmas** regras de precedência da matemática, que são:


Ordem de Precedência| Operador
:---:|:---:
1º|Expressão dentro de ( )
2º| divisão e multiplicação
3º| mod e div
4º|soma e subtração

Por isso, é de extrema importância para a corretude da sua lógica, a utilização de parênteses em cálculos onde é necessário que os operadores de menor precedência possuam maior precedência.
