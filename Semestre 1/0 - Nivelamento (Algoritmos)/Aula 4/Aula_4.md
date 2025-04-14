# Aula 4: Estruturas de repetição
## Introdução
- Imagine que estamos programando um algoritmo para exibir uma frase 5 vezes. Mas e se fossem 5000 vezes?
- As estruturas de repetição (ou **loops**) são usadas para executar um bloco de código repetidamente, enquanto uma condição específica for verdadeira ou por um determinado número de vezes.

Exemplo:
- Imagine que queremos mover um personagem de um jogo em uma plataforma até ele chegar em um item.
![](https://i.imgur.com/Uv384NB.png)
- Para pegar a moeda, nosso personagem teria que dar 10 passos. Como podemos escrever isso em um código?

- Podemos criar uma estrutura de repetição para executar a ação "andar" 10 vezes até chegar na moeda.

## Estrutura while
- O **while** (enquanto) é utilizado quando queremos que determinado código seja executado **enquanto** determinada **condição** for satisfeita.
```python
while condição
    código a ser executado
```
- Essa estrutura é geralmente acompanhada de uma **variável sentinela**. Essa variável sofre uma **alteração** durante a execução do código.

Exemplo:
```python
contador = 0

while (contador < 7):
    contador += 1
    print(contador)
```
>Saída:
1
2
3
4
5
6
7

- A variável "**contador**" é **incrementada** em **1** a cada **repetição** (**iteração**) da estrutura.
- O programa para quando a condição **contador < 7** **deixa** de ser **verdadeira**

==Pergunta==
O que esse algoritmo faz?
```python
numero = int(input("Digite um número: "))
soma = 0

while numero != 0:
    soma += numero
    numero = int(input("Digite outro número (0 para sair)"))

print(f"Soma total: {soma}")
```
> Resposta: Soma números inteiros (o valor da soma é armazenado na variável **soma**). E quando o usuário digita 0 o programa para e exibe a soma total.

## Estrutura for
- A estrutura "**for-in**" é útil para **repetir** um conjunto de comandos de maneira **contada** dentro de um **intervalo especificado**.
- A seguinte estrutura representa **uma das formas** de utilizar o **for**:
```python
for variavel in range(valorInicial, valorLimite, passo):
    Bloco de código...
```
Nesse código:
- **variavel** : variável iteradora
- **valorInicial** : opcional
- **valorInicial**, **valorLimite** : intervalo de repetição
- **passo** : incremento da variável iterada (opcional)

Exemplo 1:
```python
# Aalgoritmo que faz uma contagem de 0 até 10 de 2 em 2:

for numero in range(0, 10, 2):
    print(numero)

print("Fim")
```
> Saída:
0
2
4
6
8
Fim

Exemplo 2:
```python
# Algoritmo que imprime uma string um determinado número de vezes:

for var in range(5):
    print("Oiii")

print("Tchau!!")
```
> Saída:
Oiii
Oiii
Oiii
Oiii
Oiii
Tchau!!

Exemplo 3:
```python
# Algoritmo que imprime cada caractere de uma string:

for letra in "aeiou":
    print(letra)

print("Acabou!!")
```
> Saída:
a
e
i
o
u
Acabou!!

- Nesse caso, estamos **iterando** uma string.