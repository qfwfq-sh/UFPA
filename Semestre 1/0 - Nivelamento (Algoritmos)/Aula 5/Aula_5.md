# Aula 5: Listas
## O que é uma lista?
É um tipo de **dado** que pode armazenar um ou mais valores.

![](https://i.imgur.com/7oRiOph.png)
- Uma lista **homogênea** armazena apenas itens do **mesmo tipo**. 
- Cada item da lista possui um **indíce**.

Exemplo de lista heterogênea:
![](https://i.imgur.com/geMGrjA.png)
- Uma lista **heterogênea** pode armazenar itens de **diferentes tipos**.
- Cada item da lista possui um **índice**.

## Como acessar um ítem?
Podemos **acessar** um item de uma lista por meio de seu índice:

```python
lista = [4, 3, 5, 2]

print(lista[2])
print(lista[0])
print(lista[-1])
```
> Saída:
5
4
2

- O **índice** indica a posição de um item na lista.

## Como adicionar itens?
Em **python**, podemos **adicionar um item** à uma lista de duas formas:

```python
lista = [1, 4]

lista.append("a")
print(lista)

lista.insert(1, "ui")
print(lista)
```
> Saída:
> [1, 4, 'a']
> [1, 'ui, 4, 'a']

- **.append("item")** : Insere **item** no **final** da lista.
- **.insert(1, "item")** : Insere **item** no **índice indicado**.

## Como remover itens
Em **python**, podemos **remover um item** de uma lista de duas formas:

```python
lista = [1, "ui", 4, "a"]

lista.pop(0)
print(lista)

lista.remove(4)
print(lista)

lista.pop()
print(lista)
```
> Saída:
> ['ui', 4, 'a']
> ['ui, 'a']
> ['ui']

- **.pop(indice)** : remove **item** de acordo com o **índice**
- **.pop()** : remove o **último item** da lista
- **.remove(item)** : remove **item** de acordo com o **valor**