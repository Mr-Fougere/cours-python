	**Construction d'un code** 🏗️
- Import
- Constantes 
- Variables
- Functions 
- Instructions de code
````
===== imports ==========
import random 

====== const ==========
MONTHS = ["January",...]
YEAR = 2019

====== variables =========
name = ""
age = ""

number = ""

======= functions =====

def birthday( age ):
	instructions

def calcNumbe( number):
	instructions 

====== instructions ===== 
age = input( "Rentrez un age :")

birthday(age)

calcNumber(age)

````
---
**Type de variables** 🔢

- INTEGER ( int ) ➡️ chiffres entre 0 et infini
- STRING ( str ) ➡️ chaine de charactère 
- BOOLEAN ( bool )➡️ True / False
- ARRAY ( arr )➡️ Tableau de valeurs
- FLOAT ( float )➡️ chiffre à virgule 0.0 
---
**Opérateur arithmétique** ✖️

- a + b ➡️ additionne la valeur de a à b  ( float / int / string )
- a - b ➡️ soustrait la valeur de a à b  ( float / int )
- a / b ➡️ opére la division de a par b ( float / int)
- a %b  ➡️ obtient le reste de la division entière de a par b ( float / int )
- a // b➡️ obtient la division entière de a par b (float / int )
- a * b ➡️ obtient la multipliccation de a fois b ( float / int ou int * str )
- a ** b ➡️ obtient la puissance de a par b ( float / int )
---
 **Opérateur assignation** ✖️

- = ➡️ assigne à la variable la valeur qui suit ( float / int / arr / boolean / str )
- += ➡️ assigne à la variable l'adddition avec la valeur qui suit ( float / int )
- -= ➡️ assigne à la variable la soustraction avec la valeur qui suit ( float / int )
- /= ➡️ assigne à la variable la division avec la valeur qui suit ( float / int )
- %= ➡️ assigne à la variable le reste de la divion entière avec la valeur qui suit ( float / int )
- //= ➡️ assigne à la variable la division entière avec la valeur qui suit ( float / int )
- * = ➡️ assigne à la variable la multiplication avec la valeur qui suit ( float / int )
- ** = ➡️ assigne à la variable la puissance avec la valeur qui suit ( float / int )
---
**Opérateur logique** ➖

- x and y ➡️ Retourne vrai si x et y sont à True
- x or y ➡️ Retourne vrai si x ou t est à True
- not x ➡️ Retourne la valeur inverse de x
---
**Opérateur de comparaison** ➗

- x > y ➡️ Retourne vrai si x est supérieur à y  
- x < y ➡️ Retourne vrai si x est inférieur à y 
- x == y ➡️ Retourner vrai si x est égale à y 
- x != y➡️ Retourne vrai si x n'est pas égale à y 
- x >= y ➡️ Retourner vrai si x est supérieur ou égal à y 
- x <= y➡️ Retourner vrai si x est inférieur ou égal à y 
- x in y ➡️ Retourner vrai si x est présent dans y ( y étant un str ou un arr)
---
**Fonction Général** 🌐

- int( x ) ➡️ Transforme un float ou un str en int
- str( x ) ➡️ Transforme un int,float,bool en str 
- float( x ) ➡️ Transforme un int ou un str en float
- input( ) ➡️ Demande à l'utilisateur de rentrer une chaine de caractère 
- print( w ) ➡️ Affiche la valeur de x donner en paramètre
- len( x )➡️ Retourne la valeur en int de la longueur de x ( arr ou str )
- range( x ) ➡️ Retourne un tableau de nombre partant de 1 jusqu'a x -1
- reversed( ) ➡️ Retourner la valeur inverse d'une chaine de caractère ou d'un tableau 
---
**Fonction uniquement string** 🔡

- .replace( x , y ) ➡️ Remplace toutes les occurences de x par y 
- \[  x , y \] ( *slice* ) ➡️ Récupère la valeur correspondat à x **ou** de x jusqu'a y si y est précisé 
- .find( x ) ➡️ Retourne l'emplacement de la première occurence de x 
- .lower( ) ➡️ Retourne en minuscule la chaine de caractère
- .upper( ) ➡️ Retourne en majuscule la chaine de caractère
- .split( x ) ➡️ Découpe la chaine à chaque occurence de x et retourne un tableau de valeur correspondant aux valeurs entre chaque occurence
- .count( x ) ➡️ Retourne le nombre d'occurence de x en int 
- .index( x ) ➡️ Retourner l'emplacement de la première occurence de x ( x étant un caractère )
---
**Fonction uniquement array** 📑

- .append( x ) ➡️ Ajoute à la fin d'un tableau la valeur x 
- .count( ) ➡️ Retourne le nombre d'occurence de x dans le tableau
- .index( x ) ➡️ Retourne la position  de la première ocurrence de x dans le tableau
- .insert( x , y ) ➡️ Insère la valeur x à position y dans le tableau ( ! Remplace ou ajoute )
- .pop ( x ) ➡️ Supprime l'élément à position x dans le tableau 
- .remove ( x ) ➡️ Supprimer la première occurence x dans le tableau
---
**Condition if ..** 🔎

If est toujours suivi d'une condition utilisant un opérateur de comparaison  ou bien d'une variable dans ce dernier cas, il retournera vrai si la variable a une valeur différente de False.

````
If ( condition ) : 
	bloc d'instruction
elsif ( condition ):
	bloc d'instruction
else : // si aucune des conditions précédentes ne sont vrai passe dans celle-ci 
	bloc d'instruction
````

```
if a > b :
	print( " a est supérieur à b ")
else :
	print ( " a n'est pas supérieur à b")
```

```
if a > b :
	print( " a est supérieur à b ")
elsif a == b :
	print( " a est égale à b")
else :
	print ( " a est inférieur à b ")
```

```
if a  :
	print( " a n'est pas initialiser ")
else :
	print ( " a est initialiser ")
```

```
if a == b :
	print( " a est égale à b ")
elsif a < b :
	print ( " a est inférieur à b ")

print( " a est supérieur à b ")
```
----
 ** Boucles For 🔃** 

Une boucle for se construit grâce à une variable d'itération et d'un itérateur ( un arr ou un str).
```
For ( variable d'itération ) in ( itérateur ) : 
	instructions
```

Une syntaxe à respecter pour ne pas se perdre et de nommé toujours la variable d'itération avec le singulier du nom de l'itérateur. Sinon prendre les nom de variables préétablie à cet effet qui sont : i , j , k ,l ,m ,etc ..

```
For month in months : 
	print(month)
```

```
For call in calls : 
	print(call)
```
---
**Boucle while 🔃**

Une boucle for se construit grâce à une condition qui doit être à Vrai pour continuer à itérer sur les instructions 
```
While ( condition ) : 
	instructions
```

Il faut très attention à la condition, si aucune instructions dans la boucle ne permet de rompre la condition on crée alors une boucle infini.

```
While 1 : 
	instructions
```

```
a = 0 
While a < 10 : 
	a += 1
```
---
**Utilisation des fichiers** 📁

- open( `chemin vers le fichier` , `méthode utilisé sur le fichier `)
- méthodes :
	- "a" pour rajouter du texte à la suite
	- "r" pour récupérer le texté présent dans le fichier sous le format str
	- "w" pour surécrire sur le texte déja présente dans le fichier et le créer si le fichier n'existe pas déjà
- .readLines( ) ➡️ retourne un tableau correspondant à l'application de la fonction ``.split('/n')`` sur le fichier 
___
**Utilisation des modules🚀**

- import X➡️ import le module X en entier ( toutes les fonctions associés sont utilisables)
- from X import Y ➡️ import la fonction Y du module X ( le reste des fonctions du module ne sont pas utilisables ! )
- module.fonction ➡️ pour utiliser une fonction présente dans un module 
___ 
**Interpolation d'une chaine de caractères**

En utilisant la méthode **``f``** devant une chaine de caractère, on peut utiliser les variables présente dans le code ainsi que procéder à des instructions.
```
print( f"Tu as { age  } ans ")
```

```
print( f"Dans 10 and ,tu auras { age +10 } ans !")
```
