# Aula 3: Operadores e estruturas condicionais

## Operadores
### Operadores aritméticos
- Utilizados na execução de operações matemáticas:

|     Operação    | Símbolo  |
|     --------    | -------- |
|        Soma     |    +     |
|     Subtração   |    -     |
|   Multiplocação |    *     |
|   Exponenciação |    **    |
|      Divisão    |     /    |
| Divisão Inteira |    //    |
|Módulo da divisão|    %     |


### Operadores relacionais
- Utilizados para **comparar** dois valores:

|   Símbolo |     Significado    |
| --------- |   --------------   |
|      >    |     maior que      |
|      <    |     menor que      |
|     >=    |  maior ou igual a  |
|     <=    |  menor ou igual a  |
|     ==    |       igual a      |
|     !=    |     diferente de   |

### Operadores lógicos
- Utilizados para criar expressões lógicas:
    - **AND** (E) : Retorna verdadeiro caso **todas** as expressões sejam verdadeiras.
    - **OR** (OU) : Retorna verdadeiro caso **pelo menos uma** das duas expressões seja verdadeira.
    - **NOT** (NÃO) : Retorna o **oposto** do valor da expressão.

## Estruturas Condicionais
São estruturas utilizadas para **controlar o fluxo** de um programa.
Determina **condições** para a execução de trechos de código **específicos**.

Exemplo:
**Se** você tem 18 anos de idade ou mais, então você é maior de idade.
**Senão**, você é menor de idade.

![](https://lh3.googleusercontent.com/proxy/DPiGxtQLIN8Z8Am2Er0CX09TItMBRENgRZc-K7pd4Phi5-X4rswBuA8Tb5uEkEhVsSn2jdoDCyHJr3ZYlYZbkRzhbZxPp4i-M5CkPqiyAkEFnSy2MRcK55w)

## O que são as condições?
São representadas por **expressões lógicas** ou **relacionais** que podem ser satisfeitas ou não.

Satisfazer uma condição significa que ela recebe o valor "**True**".

## Estrutura "if-else"
Controla o **fluxo** de um programa, **escolhendo** o bloco de comandos a serem executados.

```python
if (condicao):
    ... bloco de código 1
else:
    ... bloco de código 2
```

- **if** (condicao) : estrutura condicional **"se"**.
- *bloco de código 1* : bloco de código a ser executado caso a condição seja atendida
- **else** : estrutura condicional **"senão"**
- *bloco de código 2* : bloco de código a ser executado caso a condição definida não seja atendida.

Exemplo:
```python
if (idade >= 18):
    print("Você é maior de idade!")
else:
    print("Você não é maior de idade")
```
## Estrutura "if-elif-else"
Utilizada para avaliar **mais de uma condição**.
**"elif"** é uma abreviação de **"else if"** (senão, se).

Exemplo:
```python
if (hora >= 6 and hora < 12):
    print("Bom dia!")
elif (hora >= 12 and hora < 18):
    print("Está de tarde!")
elif (hora >= 18 and hora < 0):
    print("Boa noite!")
else:
    print("Vai dormir!")
```
> **nota**: podemos utilizar tanto **operadores relacionais** quanto **operadores lógicos** para estabelecer condições.

## Indentação
É o espaço equivalente a um **"tab"** que indica quais linhas de código estão **"aninhadas"** à condição. É o **escopo** de um comando.

**Extremamente importante** para a organização do código em estruturas de condição, repetição, definição de funções e etc.