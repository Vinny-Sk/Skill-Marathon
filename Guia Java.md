Comandos Básicos

System.out.println()

O que faz: Exibe uma mensagem na tela e adiciona uma nova linha.

Exemplo: System.out.println("Hello, World!"); exibe "Hello, World!" no console.

Scanner

O que faz: Lê a entrada do usuário a partir do console.

Exemplo:

java

Copiar código

import java.util.Scanner;

Scanner scanner = new Scanner(System.in);

String nome = scanner.nextLine();  // Lê uma linha de entrada

Variáveis

O que faz: Armazena valores em memória para uso posterior.

Exemplo: int x = 5; armazena o número 5 na variável x.

Condicionais

if: Executa um bloco de código se a condição for verdadeira.

else: Executa um bloco de código se a condição do if for falsa.

Exemplo:

java

Copiar código

if (x > 0) {

System.out.println("Positivo");

} else {

System.out.println("Negativo");

}

Loops

for: Itera sobre uma sequência ou realiza um número fixo de iterações.

while: Executa um bloco de código enquanto uma condição for verdadeira.

Exemplo:

java

Copiar código

for (int i = 0; i < 5; i++) {  // Itera de 0 a 4

System.out.println(i);

}

Funções e Métodos

Definindo Métodos

O que faz: Cria um bloco de código reutilizável.

Exemplo:

java

Copiar código

public int minhaFuncao(int param) {

return param \* 2;

}

Métodos da Classe Math

Math.sqrt(): Retorna a raiz quadrada de um número.

Exemplo: double raiz = Math.sqrt(16); resulta em 4.0.

Estruturas de Dados

Arrays

O que faz: Armazena uma coleção de elementos do mesmo tipo.

Exemplo: int[] numeros = {1, 2, 3, 4};.

ArrayList

O que faz: Uma lista dinâmica que pode crescer e encolher.

Exemplo:

java

Copiar código

import java.util.ArrayList;

ArrayList<Integer> lista = new ArrayList<>();

lista.add(1);  // Adiciona o elemento 1

HashMap

O que faz: Armazena pares de chave-valor, permitindo acesso rápido.

Exemplo:

java

Copiar código

import java.util.HashMap;

HashMap<String, String> mapa = new HashMap<>();

mapa.put("chave", "valor");

Tratamento de Erros

Try/Catch

O que faz: Captura e trata exceções que podem ocorrer durante a execução do código.

Exemplo:

java

Copiar código

try {

int resultado = 10 / 0;  // Isso causará um erro

} catch (ArithmeticException e) {

System.out.println("Divisão por zero!");  // Exibe a mensagem de erro

}

Manipulação de Arquivos

Lendo Arquivos

O que faz: Permite ler o conteúdo de um arquivo.

Exemplo:

java

Copiar código

import java.io.\*;

BufferedReader reader = new BufferedReader(new FileReader("arquivo.txt"));

String linha = reader.readLine();  // Lê uma linha do arquivo

Programação Orientada a Objetos

Classes e Objetos

O que faz: Permite criar novos tipos de dados com atributos e métodos.

Exemplo:

java

Copiar código

public class MinhaClasse {

private int valor;

public MinhaClasse(int valor) {

this.valor = valor;  // Atributo da classe

}

public int metodo() {

return valor;  // Método que retorna o valor

}

}

