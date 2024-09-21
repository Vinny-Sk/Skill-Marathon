Guia rápido dos programas em Python

Print = Exibe uma informação na tela

EX: print("Hello World!")

input = Recebe dados de entrado do usuário

EX: nome = input("Qual seu nome? "). Pode declarar o tipo de variável antes do input.

* Condições:

if = se, algo só acontece se cumprir o requisito do if

EX: "if x == 6:", o programa só prossegue se o x for igual a 6

elif = mesma coisa que o if, mas como só pode ser usado um if por vez, usamos elif nos outros

else = o mesmo, mas somente quando não for utilizada nenhuma outra condição

* Laços de Repetição:

for = repete uma sequência

EX: for x range(5):

`	`print (x) fará com que mostre os números de 0 a 4, uma vez que não indicamos uma lista para ser repetida

while = enquanto uma variável cumprir o requisito, o while irá se repetir

EX: while x == 5:

`	`print ("Hello World"), enquanto x for igual a 5, ficará repetindo Hello World na tela

Função def

A palavra-chave def é usada para definir funções em Python. Uma função é um bloco de código reutilizável que pode ser chamado em qualquer lugar do programa. Vamos ver como funciona:

Estrutura Básica

python

Copiar código

def nome\_da\_funcao(parametros):

\# Código da função

return resultado

Componentes

def: Indica que você está definindo uma função.

nome\_da\_funcao: O nome que você dará à função; deve ser descritivo.

parametros: Variáveis que você pode passar para a função (opcional). Você pode ter nenhum, um ou vários parâmetros.

return: Retorna um valor da função (opcional). Se não for usado, a função retornará None por padrão.

Exemplo de Função

python

Copiar código

def soma(a, b):

resultado = a + b

return resultado

\# Chamando a função

resultado = soma(3, 5)  # resultado será 8

print(resultado)  # Exibe 8

Classe class

A palavra-chave class é usada para definir classes em Python. Classes são a base da programação orientada a objetos e permitem criar novos tipos de dados que podem conter atributos (variáveis) e métodos (funções).

Estrutura Básica

python

Copiar código

class NomeDaClasse:

def \_\_init\_\_(self, parametros):

\# Atributos da classe

self.atributo = valor\_inicial

def metodo(self):

\# Código do método

return resultado

Componentes

class: Indica que você está definindo uma classe.

NomeDaClasse: O nome da classe; por convenção, deve começar com letra maiúscula.

\_\_init\_\_: Método especial chamado de construtor, que é executado quando você cria uma instância da classe. Ele é usado para inicializar atributos.

self: Referência à instância atual da classe. Usada para acessar atributos e métodos dentro da classe.

Métodos: Funções definidas dentro da classe que podem operar nos dados da instância.

Exemplo de Classe

python

Copiar código

class Pessoa:

def \_\_init\_\_(self, nome, idade):

self.nome = nome  # Atributo da classe

self.idade = idade

def apresentar(self):

return f"Meu nome é {self.nome} e eu tenho {self.idade} anos."

\# Criando uma instância da classe

pessoa1 = Pessoa("Alice", 30)

\# Chamando um método da classe

print(pessoa1.apresentar())  # Exibe "Meu nome é Alice e eu tenho 30 anos."







