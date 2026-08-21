# Einstieg Python

## Primzahlen

Meine Lösung dieser Aufgabe sieht wie folgt aus:

```py
for z in range(1, 21):
    for i in range(1, z + 1):
        if z % i == 0:
            print('!', end=' ')
        else:
            print('.', end=' ')
    print()  # Neue Zeile nach jeder Zahl
```

Beachtenswert:
- die `range()` Funktion nimmt ganzzahlige Start- und Endwerte ein, wobei der End-Wert nicht erreicht wird. Im obigen Code nimmt die Variable `z` also nur die Werte `1..20` an, `21` wird nie zugewiesen.
- Mit dem Modulo-Operator `%` kann die Teilbarkeit geprüft werden.
- Die `print()` Funktion nimmt ein optionales Attribut `end=` entgegen, welches nach der Textausgabe hinzugefügt wird. Standardmässig ist dies eine neue Zeile.