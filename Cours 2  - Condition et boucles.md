----
### ⌛Questions cours précédents ⌛

1️⃣  Citer 5 types de variables possibles 

2️⃣  Comment récupérer le 5ème élément d'un tableau 

3️⃣  Comment attribuer à la variable A sa soustraction avec la variable B 

-----
### ☑️Partie QCM ☑️

1️⃣  Lequel de ces **opérateur** n'est pas un **opérateur de comparaison** ?
- [ ] ==
- [ ] !=
- [ ] >>
- [ ] >=

2️⃣  Quel est la **résultante** d'une **condition** ?
- [ ] un boolean
- [ ] un string 
- [ ] tout dépend de la condition
- [ ] rien

3️⃣  que **retrouve** t-on dans toutes les **boucles** ?
- [ ] un bloc d'instruction
- [ ] une itération 
- [ ] une variable 
- [ ] une condition 

4️⃣  Quand s'arrête la **boucle** suivante : ``while i>10`` :
- [ ] i est égale à 10 
- [ ] i est supérieur à 10 
- [ ] i est inférieur à 10 
- [ ] i est égale à 9  

5️⃣  Laquelle de ces **syntaxe** de boucle est **incorrect** ?
- [ ] ``while 1 :``
- [ ] ``while x == y:``
- [ ] `for i in [2,3,4]:`
- [ ] `for i > 1 :`

6️⃣   Lequel de ces **opérateurs** n'est un opérateur **logique** ?
 - [ ] and 
 - [ ] or
 - [ ] not 
 - [ ] in

7️⃣  Quels **vérites** correspond à la **validation** de la **condition** suivante : `((a >= b) and (b > 10) ) or (c != 5) ` ?
- [ ] a doit être supérieur ou égale à b  
- [ ] uniquement b doit être supérieur à 10 
- [ ] uniquement c doit être différent de 5
- [ ] a doit être inférieur ou égale à b

8️⃣  Laquelle de ces **syntaxe** ne **correspond** pas à une **condition** ?
- [ ] ``if a > b :``
- [ ] ``if a :``
- [ ] `if a==b: ; elif a==c : ; else`
- [ ] `if a or b ; else `

9️⃣  Quel est la **bonne** **syntaxe** correspond à la **phrase** suivante : a doit être supérieur à b multipler par c , ou b est égale à a au carré et c n'est pas égale à b?
- [ ] `(a > (b*c) ) or ((b == c*c) and (c != b)) `
- [ ] `(a > bc ) or (b == c*c and c != b) `
- [ ] `a > b*c or b == c*c and c != b`
- [ ] `a > (b*c) or (b == c*c) and (c != b) `

🔟  Combien d'**itération** va faire la **boucle** suivante : ``for i in range( 10 ):``? 
- [ ] 10
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

2️⃣  Que retourne l'éxécution de ce code ? 
````
i = 1

while i < 20:

	i *= 2

print( i )
````

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

4️⃣  Que permet le code suivant ? Modifier le pour qu'il soit plus explicite
````
chiffre = int ( input ("Insérer un chiffre : " ))

flag = False

for i in range(2, chiffre):

        if (chiffre % i) == 0:

            flag = True

print(not flag)
````

5️⃣  **Compléter** ce code
````
# Ce code permet à l'utilisateur de savoir si il a la majorité francaise et/ou international sinon dans combien de temps il les aura

# On demande avant tout l'âge de l'utilisateur

...... = int( input( " Veuillez indiquer votre âge :"))

# Si son age est inférieur à 18 alors on affiche dans combien de temps ils auront les deux majorités

if ..... < .... :

    print(f" Vous aurez la majorité francaise dans { ......... } ans")

    print(f" Vous aurez la majorité internationale dans { 21 - ..... } ans")

# Si son age est supérieur ou égale à 18 mais inférieur à 21 alors on affiche dans combien de temps il aura la majorité internationale.

elif ( age .... 18 ) and ( age .... 21 ):

    print(...."Vous avez la majorité francaise !")

    print(f"Vous aurez la majorité international dans { ...... } ans")

# Si il ne rempli pas les conditions précédente cela veux donc dire qu'il a 21 ans et plus il a donc les deux majorités

..... :

    print("Vous avez la majorité francaise et international. Félicitations !")
````

----
### 🏗 Partie application 🏗

Ecrire un **programme** de ✌️✊✋( pierre papier ciseaux) grâce au module random 

⭐ **Bonus** ⭐
Ecrire un **programme** reprenant le principe du **juste prix** dans une intervalle de 100 avec un nombre d'essai limité 🎰
