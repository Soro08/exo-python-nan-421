# Les class


## Declaration et appel

```python 

class Operation:
    def __init__(self):
        pass

    def somme(self, a, b):
        return a + b


# creer une nouvelle instance de la class Operation
newop = Operation()

# Output: <function Operation.somme>
print(Operation.somme(10,30))


``` 

## TP Class Python

### Exercice 1

Écrivez une classe `Domino` pour représenter une pièce de domino. Les objet sont
initialisés avec les valeurs des deux faces, A et B. Ajoutez une méthode `.affiche_points()` qui
affiche les valeurs des deux faces, et une méthode `.totale()` qui retourne la somme de deux
valeurs.

```python 
>>> d = Domino(4, 6)
>>> d.affiche_points()
face A: 4, face B: 6
>>> x = d.totale()
>>> print(x)
10
``` 
### Exercice 2

Écrivez une classe `CompteBancaire`. Les objets sont initialisés avec le nom du titulaire et le solde. L’argument solde doit être facultatif et avoir une valeur prédéfinie zéro. Ajoutez
deux méthodes `.depot(somme)` et `.retrait(somme)` pour changer le solde. Ajoutez une méthode
`.affiche()` qui montre le solde courant.

```python
>>> compte1 = CompteBancaire(’Jean’, 1000)
>>> compte1.retrait(200)
>>> compte1.affiche()
Le solde du compte de Jean est 800 euros.
>>> compte2 = CompteBancaire(’Marc’)
>>> compte2.depot(500)
>>> compte2.affiche()
Le solde du compte de Marc est 500 euros.
``` 

### Exercice 3

Generateurs. Écrivez une classe `TableMultiplication` qui crée des objets initialisés
avec un nombre entier. Ajouter une méthode `.prochain()` qui renvoie à chaque appel un nouveau
terme de la table de multiplication correspondante.

```python 
>>> tab = TableMultiplication(3)
>>> tab.prochain()
0
>>> tab.prochain()
3
>>> tab.prochain()
6
>>> tab.prochain()
9
```
### Exercice 4

Écrivez une classe `Fraction` qui crée des objets initialisés avec deux nombres entiers
`.num` et `.denom` pour le numérateur et le dénominateur. Ajoutez une méthode `.affiche()` qui
affiche une représentation de la fraction. Ajoutez des méthodes spéciales pour pouvoir utiliser les
opérateurs `+, -, *, /`.
Pour réduire la fraction, vous pouvez employer la fonction `math.gcd(a, b)` du module math, qui
calcule le plus grand commun diviseur entre deux entiers a et b.

```python
>>> f = Fraction(3, 4)
>>> f.affiche()
3/4
>>> g = Fraction(1, 2)
>>> g.affiche()
1/2
>>> r1 = f + g
>>> r.affiche()
5/4
>>> r2 = f / g
>>> r2.affiche()
3/2
```
### Exercice 6

On se propose de représenter les polynômes en une indéterminée avec un nombre
quelconque de termes :

e^{i\pi} = -1
