# Lógica de Programação com Java

## Introdução

## Sobre o Java

### Estrutura de um programa Java

```java
public class MeuApp {

    // Comentário

    /* Outro comentário */

    /* Exemplo
de comentário de
    várias linhas */

    // Método chamado assim que o programa inicia
    public static void main(String[] args) {
        // Meu código
    }
}


```

## Comentários

Comentários são trechos do código que não são executados. Eles
servem como anotações para os desenvolvedores.

Existem basicamente três tipos de comentário em Java:

Comentário de uma linha:
```java
// exemplo de comentário
System.out.println("Hello World!"); // Imprime na tela
```

Comentário de várias linhas:
```java
/* exemplo de comentário de várias

linhas
*/
System.out.println("Hello World!");
```

Existe também o docstring (denotado por /** e **/), que é usado de forma mais estruturada para documentação do código. Não precisa se preocupar com eles nesse momento.


## Imprimindo coisas na tela

Uma das ações mais simples que um programa pode fazer é escrever alguma
coisa para o usuário. Chamamos isso de saída ou output.

A forma mais simples de se imprimir algo na tela é pelos métodos print e println (não se assuste com o tamanho do comando).

```java
// O println insere uma quebra de linha (\n) no final da mensagem

System.out.println("Hello World!");

// Imprimindo sem quebrar linha

System.out.print("Aba");
System.out.print("cate");

// Quebrando linha manualmente

System.out.print("Quebrando a linha\n");
System.out.print("manualmente");

/* Saída:
Hello World!
Abacate
Quebrando a linha
manualmente
*/
```

## Variáveis

### O que são

Variáveis não são nada mais do que espaços na memória do computador que seu programa pode usar pra trabalhar. As variáveis dentro de um programa geralmente têm nomes descritivos, que dizem o que elas "carregam".

```java
String nome = "Agata";
int idade = 22;
double saldoNaConta = 9999.99;
```

Lembre-se de quando você preenche um formulário para se cadastrar em um site. Cada um dos campos, como nome, data de nascimento, endereço, email, etc, entra como uma variável para o programa do site. O site pode internamente fazer operações e jogar em variáveis internas (ex: calcular sua idade e jogar em uma variável idade) e ter variávels de saída, como uma mensagem do tipo "cadastrada com sucesso" ou "Erro ao cadastrar"

Para criarmos uma variável, primeiro declaramos o tipo dela, em seguida seu nome e, opcionalmente, atribuímos algum valor a ela.

Futuramente, podemos também sobrescrever o valor de uma variável.

Ex:

```java
int meuNumero = 42;

System.out.println("meuNumero é " + meuNumero);

meuNumero = 98;

System.out.println("meuNumero agora é " + meuNumero);

/*
meuNumero é 42
meuNumero agora é 98
*/
```

### Tipos de dados

No Java, sempre que você declara uma variável, você tem que dizer para ele que tipo de dado ela vai carregar (afinal, ele tem que reservar espaço na memória para ela).

Os tipos básicos de dados são:

#### Tipos primitivos

##### char
Caracteres simples, delimitados por aspas simples.

Existem alguns caracteres especiais, como '\n' (quebra de linha), '\t' (tab).

Caso você precise escrever ' ou \ em um char, pode escrever como '\'' e '\\', respectivamente. Essa lógica também se aplica a String, que usam " (vira "\"").

Exemplos:

'a', 'z', '0', '9', '\n', '\t'

##### byte, short, int e long

Representam números inteiros negativos e positivos.
Suas diferenças estão nos quanto ocupam em memória e nos seus limites.

Por padrão, ao simplesmente digitar um número, o Java o interpreta como um int

Os limites de cada um deles com exemplos pode ser encontrado [aqui](https://www.baeldung.com/java-primitives)

##### float e double

Representam valores "quebrados", como 0.5, 0.226, -58.3, etc. 

Dê preferência a usar double, já que ele é mais preciso do que o float.

##### boolean

Tipo simples, mas extremamente úteis no dia-a-dia. Podem assumir apenas dois valores: true ou false.

### Strings

Strings são basicamente vários chars seguidos (cadeia de caracteres) e são representadas por aspas duplas.

Lembra do System.out.println? Ele foi construído para receber uma String e apresentar ela na tela, e foi exatamente isso que fizemos quando escrevemos "Hello World!!" lá em cima.

### Objetos

Além disso, variáveis também podem guardar coisas maiores! Podemos guardar objetos em variáveis, por exemplo, o LocalDateTime, objeto que representa data e hora, e o próprio String.
Futuramente, poderemos criar nossos próprios objetos também.

Ao contrário dos tipos primitivos, variáveis que guardam objetos podem não ter um valor definido. Isso é representado pelo `null`.

```java
Long id = 1L;
String nome = "Agata";
int idade = 22;
LocalDateTime dataCadastro = LocalDateTime.now();

String mensagem = "Bom diaaa \\o/";

System.out.println("id: " + id + "\n" +
        "nome: " + nome + "\n" +
        "idade: " + idade + "\n" +
        "dataCadastro: " + dataCadastro + "\n");

System.out.println("_/\\/\\__" + mensagem + "-_/\\/\\_");

\*
id: 1
nome: Agata
idade: 22
dataCadastro: 2021-04-01T00:36:34.140774

_/\/\__Bom diaaa \o/-_/\/\_
*/

```

## Operadores e Lógica Booleana

### Operadores Aritméticos

| Operador                  | Sinal     | Exemplo               | Obs |
| --------------------------|-----------|-----------------------|-------------|
| Adição                    | +         | x + y                 | Também pode ser usado para juntar (concatenar) Strings
| Subtração                 | -         | x - y                 |
| Multiplicação             | *         | x * y                 |
| Divisão                   | /         | x / y                 | 
| Resto da divisão inteira  | %         | x % y                 | 5 % 4 = 1 (resto da divisão)
| Sinal positivo            | +         | +x                    | +(1) = 1; +(-1) = -1
| Sinal negativo            | +         | -x                    | -(1) = -1; -(-1) = 1
| Incremento e decremento   | ++ e --   | x++, ++x, x-- e --x   | Aumenta ou diminui em 1


## Input e Output

## Estruturas condicionais

### If

### If com else

### Ifs encadeados

### Switch case

## Laços de repetição

### Laço for

### while e do while

## Vetores (Arrays)

## Listas dinâmicas

## Tratamento de exceções



## Funções

### O que é uma função e para que serve?

Uma função serve para facilitar o nosso código. Existem vários momentos na
programação em que precisaremos reutilizar um código já criado anteriormente, para isso podemos colocar esta parte do código dentro de uma função e utiliza-la várias vezes no código inteiro, sem precisarmos ficar rependo o código.

### Estrutura de uma função

## Strings

### Caracteres especiais e de escape

### Percorrendo Strings

### Funções úteis

## Orientação a objetos

### O que é e por que é usada

### Classes e instâncias

### Importando, instanciando e utilizando classes

### Métodos de classe (estáticos)