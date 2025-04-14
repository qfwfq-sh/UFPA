# Aula 2: Variáveis, entrada e saída de dados

## O que são variáveis?
São elementos que permitem que o programador guarde e represente informações. Como se fosse uma caixinha que pode guardar vários tipos de informação. Ou um copo que pode armazenar materiais diferentes.

Para declarar uma variável **em python**, seguimos a seguinte estrutura:
```python
idade = 19
```
- idade : nome da variável
- = : sinal de atribuição
- 19 : valor que queremos atribuir à variável

Em Python, **não** é necessário declarar o **tipo** da variável.

Outro exemplo em C++:
```cpp
string txt = "oii"
```
- string : tipo da variável
- txt : nome da variável
- "oii" : valor que queremos atribuir à variável

### Tipos de variáveis:
- Inteiro (int): Valores inteiros
    3, -10, 28, 150
- Ponto flutuante (float): Números decimais
    3.14, 2.5, 1.74
- String (str): Sequências de caracteres
    "palavras", "frases", "caracteres", "10", "3.1415"
- Booleano (bool): Valores lógicos
    verdadeiro **(True)** ou falso **(False)**

O que é um valor **booleano**?
Uma variável pode assumir **apenas dois** valores (ou estados):
- **True**: Um valor verdadeiro;
- **False** Um valor falso;

Observações:
---
- Os nomes devem ser **claros e objetivos** para maior legibilidade;
- Caracteres especiais **não podem** ser usados para declarar uma variável (exceto underline);
- O nome da variável não pode começar com um número;
- O nome de variáveis é **case sensitive**
- Não pode conter espaços

Exemplos do que **não fazer**:
```python
!nome = "João"
1pi = 3.14
minha idadde = 19
```
## Entrada e saída de dados
### Entrada de dados
Como podemos **receber** um dado?
- função **input()**: Usada para receber informações do usuário.

Exemplo:
```python
nome = input("Qual é o seu nome?" )
```
- nome : variável que queremos atribuir o valor
- input : função para entrada de dados
- "Qual é o seu nome" : mensagem para o usuário

#### Tipos de variáveis no input
- Todo dado recebido por um input é uma string;
- Podemos "escolher" o tipo da variável que queremos receber.

Exemplo:
```python
idade1 = input("Qual é a sua idade?" )
> 20
# (tipo: string - "20")

idade2 = int(input("Qual é a sua idade? ")) 
> 23.4
# (tipo: int - 23)
```
É útil para garantir que estamos trabalhando com o **tipo correto** de dados!

## Saída de dados 
Como podemos **mostrar** um dado?
- função print(): Usada para mostrar informações ao usuário.

Exemplo:
```python
print("Hello, World!")

# ou

print(3.1415)
```

- print : função para saída de dados
- "Hello, world!" e 3.1415 : dado que queremos exibir

```python
mensagem = input("Digite uma mensagem: ")
print(mensagem)
```
Saída:
\> Digite uma mensagem: **Olá mundo**
\> Olá, mundo!

### Função print() - f-strings
- Permitem que variáveis sejam **formatadas** dentro da mensagem do **print()**
- Ajuda na organização da saída do código
- Basta colocar a letra "f" antes do texto e o nome da variável entre chaves {}.

Exemplo:
```python
nome = "Maria"
idade = 18

print(f"{nome} tem {idade} anos.")
```
\> saída: Maria tem 18 anos.

> Obs: Você pode "somar" e "multiplicar" (concatenar) strings!
> Ex: "oi, " + "tudo bem?" = "oi, tudo bem?"

## Tipagem de dados
- **Tipagem estática**: A linguagem **não permite** que o programador **altere** o tipo de uma variável ao longo da execução de um programa.
- **Tipagem dinâmica**: A linguagem **permite** que o programador **altere** o tipo de uma variável ao longo da execução de um programa.
- *Tipagem forte*: A linguagem realiza a **inferência de tipos** automaticamente.
- *Tipagem fraca*: A linguagem **não** realiza a **inferência de tipos** automaticamente.

==Python é uma linguagem de **tipagem dinâmica** e **forte**==