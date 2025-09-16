# 📊 Datenstrukturen

## Listen

Wir alle kennen Listen aus dem Alltag wie z.B. eine **Einkaufsliste** beim Shopping, eine **Kontaktliste** auf dem Smartphone oder eine **To-Do-Liste** mit Aufgaben, die wir erledigen wollen.

In all diesen Listen werden Elemente **in einer bestimmten Reihenfolge** gespeichert. Sie werden durch eckige Klammern `[]`gekennzeichnet. Hier ein Beispiel:

```python
shopping_list = ["banana", "cornflakes", "chicken", "bread", "soap"]

print(type(shopping_list))      # <class 'list>'
```

In dieser Einkaufliste sind mehrere Elemente mit dem Datentyp **String** gespeichert (Merke: Listen können auch mit Elementen verschiedener Datentypen gefüllt werden). Die Konsole gibt ausserdem den **Datentypen** von `shopping_list` aus und erkennt diese als **Liste**.

```python
shopping_list = ["banana", "cornflakes", "chicken", "bread", "soap"]

print(type(shopping_list))      # <class 'list>'
```

Um die Anzahl der Elemente in einer Liste zu bestimmen, kann man die Funktion `len()` verwenden.

```python
len(shopping_list)      # Ergibt 5, weil 5 Elemente in der Liste gespeichert sind.
```

In einer Liste hat jedes Elemente seine Position, die als **Index** ausgedrückt wird. Das erste Element einer Liste hat den **Index 0**. Wenn wir ein bestimmtes Element einer Liste auslesen wollen, schreiben wir einfach den Index in die eckigen Klammern.

```python
meat = shopping_list(2)

print(meat)     # Ausgabe: "chicken"
```
Wenn wir wissen möchten, welchen Index ein bestimmtes Element in einer Liste hat, brauchen wir die Methode `index()`.

```python
position_bread = shopping_list.index("bread")
print(position_bread)                           # Ausgabe: 3
```

Um Elemente innerhalb einer Liste zu sortieren, können wir die Methode `sort()` verwenden. Sie sortiert Zahlen und Zeichenketten in **aufsteigender Reihenfolge** (z.B. von 0 bis 10, oder von a bis z). Das funktioniert aber nur, wenn die Elemente in einer Liste vom gleichen Datentypen sind.

Wollen wir Elemente in **absteigender Reihenfolge** sortieren, ergänzen wir das Keyword-Argument `reverse=True`.

```python
shopping_list.sort()

print(shopping_list)    # ['banana', 'bread', 'chicken', 'cornflakes', 'soap']

shopping_list.sort(reverse=True)

print(shopping_list)    # ['soap', 'cornflakes', 'chicken', 'bread', 'banana']
```

Wenn wir wissen wollen, **wie oft** ein bestimmtes Element in einer Liste auftaucht, kann man die Methode `count()` verwenden.

```python
todo_list = ["yoga", "shopping", "study", "lunch", "yoga", "coding", "dinner", "yoga"]

amount = todo_list.count("Yoga")
print(amount)                       # 3
```

Eine Liste ist dynamisch aufgebaut und hat keine feste Grösse. Wir können beliebig Elemente **entfernen** oder **hinzufügen**.

```python
numbers = [0, 1, 2, 3, 4, 5]

numbers.remove(3)
print(numbers)                       # [0, 1, 2, 4, 5]

numbers.append(2)
print(numbers)                       # [0, 1, 2, 4, 5, 2] Das neue Element wird zuhinterst an die Liste angehängt.
```
