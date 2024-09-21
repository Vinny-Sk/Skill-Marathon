O Que é Programação Orientada a Objetos (POO)?

A Programação Orientada a Objetos é um paradigma que utiliza "objetos" para representar dados e comportamentos. Os principais conceitos da POO incluem:

Classes: Moldes que definem a estrutura e o comportamento de objetos, encapsulando dados e métodos.

Objetos: Instâncias de classes que possuem estado (atributos) e comportamento (métodos).

Encapsulamento: Protege o estado interno de um objeto, controlando o acesso aos seus atributos e métodos.

Herança: Permite que uma classe herde características de outra, promovendo a reutilização de código.

Polimorfismo: Permite que objetos de diferentes classes sejam tratados como objetos de uma classe comum.

Estrutura de Classes em Python

Definindo uma Classe

A definição de uma classe em Python envolve a declaração da classe, seus atributos e métodos.

python

Copiar código

class NomeDaClasse:

def \_\_init\_\_(self, parametro1, parametro2):

self.atributo1 = parametro1

self.atributo2 = parametro2

def metodo(self):

\# Código do método

pass

Exemplo Prático

Vamos considerar um exemplo de uma classe Carro.

python

Copiar código

class Carro:

def \_\_init\_\_(self, modelo, cor):

self.modelo = modelo

self.cor = cor

self.ligado = False  # Estado inicial

def ligar(self):

self.ligado = True

print(f"{self.modelo} está ligado.")

def desligar(self):

self.ligado = False

print(f"{self.modelo} está desligado.")

Usando a Classe

Você pode criar instâncias da classe e usar seus métodos:

python

Copiar código

carro1 = Carro("Fusca", "azul")

carro2 = Carro("Civic", "preto")

carro1.ligar()  # Exibe "Fusca está ligado."

carro2.ligar()  # Exibe "Civic está ligado."

carro1.desligar()  # Exibe "Fusca está desligado."

Encapsulamento

O encapsulamento em Python é realizado usando convenções de nomenclatura. Por exemplo, atributos prefixados com um underscore (\_) indicam que devem ser tratados como privados.

Exemplo de Encapsulamento

python

Copiar código

class ContaBancaria:

def \_\_init\_\_(self, saldo\_inicial):

self.\_saldo = saldo\_inicial  # Atributo "protegido"

def depositar(self, valor):

self.\_saldo += valor

def mostrar\_saldo(self):

print(f"Saldo: {self.\_saldo}")

Herança

A herança permite que uma nova classe herde atributos e métodos de uma classe existente, facilitando a reutilização de código.

python

Copiar código

class Veiculo:

def \_\_init\_\_(self, modelo):

self.modelo = modelo

def mover(self):

print(f"{self.modelo} está se movendo.")

class Carro(Veiculo):  # Carro herda de Veiculo

def \_\_init\_\_(self, modelo, cor):

super().\_\_init\_\_(modelo)  # Chama o construtor da classe base

self.cor = cor

def mostrar\_cor(self):

print(f"Cor do carro: {self.cor}")

Polimorfismo

O polimorfismo permite que você trate diferentes tipos de objetos de forma uniforme. Em Python, isso é frequentemente feito através de métodos que têm o mesmo nome, mas comportamentos diferentes.

python

Copiar código

class Ave:

def fazer\_som(self):

print("Som de ave")

class Pato(Ave):

def fazer\_som(self):

print("Quack")

class Canario(Ave):

def fazer\_som(self):

print("Tweet")

\# Uso do polimorfismo

def emitir\_som(ave):

ave.fazer\_som()

pato = Pato()

canario = Canario()

emitir\_som(pato)    # Exibe "Quack"

emitir\_som(canario) # Exibe "Tweet"

Resumo

Classes: Moldes que definem objetos com atributos e métodos.

Objetos: Instâncias de classes, que mantêm estado e comportamento.

Encapsulamento: Protege dados através de convenções de nomenclatura.

Herança: Permite que classes herdem atributos e métodos de outras classes.

Polimorfismo: Permite que diferentes classes implementem métodos com o mesmo nome de maneiras distintas.
