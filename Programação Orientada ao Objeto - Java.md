* ﻿O Que é Programação Orientada a Objetos (POO)?

* A Programação Orientada a Objetos é um paradigma de programação que utiliza "objetos" para representar dados e métodos que operam sobre esses dados. Os principais conceitos da POO incluem:

* Classes: São moldes que definem a estrutura e o comportamento de objetos. Elas encapsulam dados e métodos.

* Objetos: Instâncias de classes que possuem estado (atributos) e comportamento (métodos).

* Encapsulamento: Protege o estado interno de um objeto, controlando o acesso aos seus atributos e métodos.

* Herança: Permite que uma classe herde características de outra classe, promovendo a reutilização de código.

* Polimorfismo: Permite que objetos de diferentes classes sejam tratados como objetos de uma classe comum, geralmente através de métodos sobrescritos.

* Estrutura de Classes em Java

* Definindo uma Classe

A definição de uma classe em Java inclui a declaração da classe e seus atributos e métodos.

java


public class NomeDaClasse {

// Atributos

private Tipo atributo1;

private Tipo atributo2;

// Construtor

public NomeDaClasse(Tipo parametro1, Tipo parametro2) {

this.atributo1 = parametro1;

this.atributo2 = parametro2;

}

// Métodos

public void metodo() {

// Código do método

}

}

* Exemplo Prático

Vamos considerar um exemplo de uma classe Carro.

java

public class Carro {

// Atributos

private String modelo;

private String cor;

private boolean ligado;

// Construtor

public Carro(String modelo, String cor) {

this.modelo = modelo;

this.cor = cor;

this.ligado = false; // Estado inicial

}

// Métodos

public void ligar() {

ligado = true;

System.out.println(modelo + " está ligado.");

}

public void desligar() {

ligado = false;

System.out.println(modelo + " está desligado.");

}

}

* Usando a Classe

Você pode criar instâncias da classe e usar seus métodos:

java


public class Main {

public static void main(String[] args) {

Carro carro1 = new Carro("Fusca", "azul");

Carro carro2 = new Carro("Civic", "preto");

carro1.ligar();  // Exibe "Fusca está ligado."

carro2.ligar();  // Exibe "Civic está ligado."

carro1.desligar();  // Exibe "Fusca está desligado."

}

}

* Encapsulamento

O encapsulamento em Java é realizado por meio de modificadores de acesso:

private: Atributos ou métodos são acessíveis apenas dentro da própria classe.

public: Atributos ou métodos são acessíveis de qualquer lugar.

protected: Atributos ou métodos são acessíveis na própria classe e em subclasses.

* Exemplo de Encapsulamento

java



public class ContaBancaria {

private double saldo; // Atributo privado

public ContaBancaria(double saldoInicial) {

this.saldo = saldoInicial;

}

public void depositar(double valor) {

saldo += valor;

}

public void mostrarSaldo() {

System.out.println("Saldo: " + saldo);

}

}

* Herança

A herança permite que uma nova classe herde atributos e métodos de uma classe existente, facilitando a reutilização de código.

java



public class Veiculo {

protected String modelo;

public Veiculo(String modelo) {

this.modelo = modelo;

}

public void mover() {

System.out.println(modelo + " está se movendo.");

}

}

public class Carro extends Veiculo { // Carro herda de Veiculo

private String cor;

public Carro(String modelo, String cor) {

super(modelo); // Chama o construtor da classe base

this.cor = cor;

}

public void mostrarCor() {

System.out.println("Cor do carro: " + cor);

}

}

* Polimorfismo

O polimorfismo permite que você trate diferentes tipos de objetos de forma uniforme. Em Java, isso é comumente feito usando métodos sobrescritos.

java


public class Ave {

public void fazerSom() {

System.out.println("Som de ave");

}

}

public class Pato extends Ave {

@Override

public void fazerSom() {

System.out.println("Quack");

}

}

public class Canario extends Ave {

@Override

public void fazerSom() {

System.out.println("Tweet");

}

}

// Uso do polimorfismo

public class Main {

public static void main(String[] args) {

Ave ave1 = new Pato();

Ave ave2 = new Canario();

ave1.fazerSom(); // Exibe "Quack"

ave2.fazerSom(); // Exibe "Tweet"

}

}

* Resumo

Classes: Estruturas que definem objetos com atributos e métodos.

Objetos: Instâncias de classes, que mantêm estado e comportamento.

Encapsulamento: Protege dados com modificadores de acesso.

Herança: Permite que classes herdem atributos e métodos de outras classes.

Polimorfismo: Permite que diferentes classes implementem métodos com o mesmo nome de maneiras distintas.
