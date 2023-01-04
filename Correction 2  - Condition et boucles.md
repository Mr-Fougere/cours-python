----
### ⌛Questions cours précédents ⌛

1️⃣  Citer 5 types de variables possibles 

**Réponse** :
int , string , float , array et bool

2️⃣  Comment récupérer le 5ème élément d'un tableau 

**Réponse :**
tableau[4] => tableau [ position voulu - 1]

3️⃣  Comment attribuer à la variable A sa soustraction avec la variable B 

**Réponse** : 
a -= b

-----
### ☑️Partie QCM ☑️

1️⃣  Lequel de ces **opérateur** n'est pas un **opérateur de comparaison** ?
- [ ] ==
- [ ] !=
- [x] >>
- [ ] >=

2️⃣  Quel est la **résultante** d'une **condition** ?
- [x] un boolean
- [ ] un string 
- [ ] tout dépend de la condition
- [ ] rien

3️⃣  que **retrouve** t-on dans toutes les **boucles** ?
- [x] un bloc d'instruction
- [ ] une itération 
- [ ] un opérateur de comparaison 
- [x] une condition 

4️⃣  Quand s'arrête la **boucle** suivante : ``while i>10`` :
- [x] i est égale à 10 
- [ ] i est supérieur à 10 
- [ ] i est inférieur à 10 
- [ ] i est égale à 9  

5️⃣  Laquelle de ces **syntaxe** de boucle est **incorrect** ?
- [ ] ``while 1 :``
- [ ] ``while x == y:``
- [ ] `for i in [2,3,4]:`
- [x] `for i > 1 :`

6️⃣   Lequel de ces **opérateurs** n'est un opérateur **logique** ?
 - [ ] and 
 - [ ] or
 - [ ] not 
 - [x] in

7️⃣  Quels **vérites** correspond à la **validation** de la **condition** suivante : `((a >= b) and (b > 10) ) or (c != 5) ` ?
- [x] a doit être supérieur ou égale à b  
- [ ] uniquement b doit être supérieur à 10 
- [x] uniquement c doit être différent de 5
- [ ] a doit être inférieur ou égale à b

8️⃣  Laquelle de ces **syntaxe** ne **correspond** pas à une **condition** ?
- [ ] ``if a > b :``
- [ ] ``if a :``
- [ ] `if a==b: ; elif a==c : ; else`
- [x] `if a or b ; else `

9️⃣  Quel est la **bonne** **syntaxe** correspond à la **phrase** suivante : a doit être supérieur à b multipler par c , ou b est égale à a au carré et c n'est pas égale à b?
- [x] `(a > (b*c) ) or ((b == c*c) and (c != b)) `
- [ ] `(a > bc ) or (b == c*c and c != b) `
- [ ] `a > b*c or b == c*c and c != b`
- [ ] `a > (b*c) or (b == c*c) and (c != b) `

🔟  Combien d'**itération** va faire la **boucle** suivante : ``for i in range( 10 ):``? 
- [x] 10
- [ ] 11
- [ ] 0 , il y a une erreur
- [ ] 9

----
### 📝 Partie correction pratique 📝

1️⃣  Ce code va t'il correctement s'éxécuté ? Si non pourquoi ?
````
while 1 : 
	
	print("Tout va bien")

print("Tout va mal")
````
**Réponse :**
	Le code va éxécuter en boucle la fonction ``print ( "Tout va bien ")`` car la condition du while restera vrai tout le temps.
	Le `print("Tout va mal")` ne s'effectuera jamais 

2️⃣  Que retourne l'éxécution de ce code ? 
````
i = 1

while i < 20:

	i *= 2

print( i )
````
**Réponse :**
L'éxécution va retourner la valeur de 32. Le code multiplie la valeur de i par 2 à chaque itération jusqu'a ce que i soit supérieur ou égale à 20. Au bout de la 5ème itération , i vaut 32 la condition du while n'est donc plus rempli et la boucle s'arrête. 

3️⃣ De quel facon peut-on simplifier le code suivant ?
````
personnel_autorise = ["Julie","Clément","Elodie","Pierre"]

prenom =  input( "Veuillez indiquer votre nom :")

autorisé = False

for i in personnel_autorise :

    if i == prenom:

        autorisé = True

if autorisé :

    print( f"Bienvenue { prenom }! Vous pouvez entrer ..." )

else:

    print( "Accés refusé vous ne faites pas parti du personnel autorisé !" )
````
Réponse : 

````
personnel_autorise = ["Julie","Clément","Elodie","Pierre"]

prenom =  input( "Veuillez indiquer votre nom :")

autorisé = False

// modification
if prenom in personnel_autorise :
	
	autorisé = True
// 

if autorisé :

    print( f"Bienvenue { prenom }! Vous pouvez entrer ..." )

else:

    print( "Accés refusé vous ne faites pas parti du personnel autorisé !" )
````

4️⃣  Que permet le code suivant ? Modifier le pour qu'il soit plus explicite
````
chiffre = int ( input ("Insérer un chiffre : " ))

flag = False

for i in range(2, chiffre):

        if (chiffre % i) == 0:

            flag = True

print(not flag)
````
**Réponse :**
Le code précédent permet de savoir si le chiffre rentrait par l'utilisateur est un chiffre primaire.
Pour faire cela , on vérifie si le reste de la division par chaque chiffre entre 2 et le chiffre -1 n'est pas égale à 0. Si c'est le cas, la variable flag passe à True pour nous signaler que le chiffre entré a été au moins divisé une fois .
````
chiffre = int ( input ("Entrez un chiffre pour savoir si c'est un nombre primaire : " ))

flag = False

for i in range(2, chiffre):

        if (chiffre % i) == 0:

            flag = True

if flag :
	print( f"{chiffre} est un nombre primaire !" )
else:
	print( f"{chiffre} n'est pas un nombre primaire !" )
````

5️⃣  **Compléter** ce code
````
# Ce code permet à l'utilisateur de savoir si il a la majorité francaise et/ou international sinon dans combien de temps il les aura

# On demande avant tout l'âge de l'utilisateur

age = int( input( " Veuillez indiquer votre âge :"))

# Si son age est inférieur à 18 alors on affiche dans combien de temps ils auront les deux majorités

if age < 18 :

    print(f" Vous aurez la majorité francaise dans { 18-age } ans")

    print(f" Vous aurez la majorité internationale dans { 21 - age } ans")

# Si son age est supérieur ou égale à 18 mais inférieur à 21 alors on affiche dans combien de temps il aura la majorité internationale.

elif ( age >= 18 ) and ( age < 21 ):

    print("Vous avez la majorité francaise !")

    print(f"Vous aurez la majorité international dans { 21 - ans } ans")

# Si il ne rempli pas les conditions précédente cela veux donc dire qu'il a 21 ans et plus il a donc les deux majorités

else :

    print("Vous avez la majorité francaise et international. Félicitations !")
````

----
### 🏗 Partie application 🏗

Ecrire un **programme** de ✌️✊✋( pierre papier ciseaux) grâce au module random 

⭐ **Bonus** ⭐
Ecrire un **programme** reprenant le principe du **juste prix** dans une intervalle de 100 avec un nombre d'essai limité 🎰

```
import random

print("Bienvenue! Au cours de ce programme nous vous demanderons de devinez le juste prix d'un objet")
juste_prix = random.randint(0,100)

choice = False

while choice != juste_prix:

    choice = int(input("Vueillez saisir un prix  0 et 100 :"))

    if choice > juste_prix:

        print("Moins")

    elif choice < juste_prix:

        print("Plus")

    else:

        print("Bien joué")`
```