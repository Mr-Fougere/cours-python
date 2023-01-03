-----
### ☑️Partie QCM ☑️

1️⃣ Comment **peut-on décrire** une **variable** ?
- [x] Un conteneur stockant une valeur fixe 
- [x] Un conteneur dont la valeur peut être modifé
- [ ] Elle peut avoir plusieurs type de valeur simultanément 
- [x] Il est obligatoire de lui attribuer une valeur avant d'effectuer des opérations avec celle-ci

2️⃣ Lesquels de ces **types** peut être **attribué** à une **variable** ?
- [x] int 
- [x] float 
- [x] string
- [x] bool 

3️⃣ Quel **fonction** utiliser pour convertir **"0"** en **0**  ?
- [x] int()
- [ ] string()
- [ ] number()
- [ ] integer()

4️⃣ Lequel de ces **opérateurs** n'est pas un **opérateur arithmétique** ?
- [ ] +
- [ ] **
- [x] =
- [ ] %

5️⃣ Quel **opérateur** utilisé pour avoir le **reste** qu'une **division** entre **a** et **b** ?
- [ ] a/b
- [ ] a%b
- [x] a//b
- [ ] a\*b

6️⃣ Quel **opérateur** permet d'attribuer à **c** le résultat de la **puissance** de **c** par **x**  ?
 - [ ] c += x
 - [ ] c %= x
 - [x] c \*\*= x
 - [ ] c \*= x

7️⃣ Quel **fonction** utilisé pour afficher la variable **a** ?
- [ ] show(a)
- [ ] display(a) 
- [ ] input(a)
- [x] print(a)

8️⃣ Comment demander une variable **b** à l'utilisateur ?
- [x] b = input("Indiquer b :")
- [ ] b = give("Indiquer b :")
- [ ] b = send("Indiquer b :")
- [ ] b = indicate("Indiquer b :")

9️⃣ Comment créer un **tableau de valeurs** ?
- [ ] tableau = 1 2 3 4
- [x] tableau = [ 1 , 2 , 3 , 4 ]
- [ ] tableau = [ 1 2 3 4 ]
- [ ] tableau = { 1 : 2 : 3 :4 }

🔟 Comment récupérer le **dernier élément** du **tableau** précédént  ? 
- [ ] tableau[0]
- [ ] tableau[1]
- [x] tableau[-1]
- [ ] tableau[x]

----
### 📝 Partie correction pratique 📝

1️⃣ Ce code va t'il **correctement** **s'éxécuté** ? Si non **pourquoi** ?
````
b = 0
b = a
print ( a )
````

**Réponse** : 
Non le code ne va pas s'éxécutait correctement car la variable a n'est pas attribué auparavant il est donc impossible de change la valeur de b pour a.

2️⃣ Que retourne l'**éxécution** de ce **code** ? 
````
a = 0 ; b = 3 ; c = 4 ; d = 10
tableau = [ a , b , c , d ]
résultat = tableau [ -1 ] \*\*2
résultat /= tableau [ b ]
print( résultat )
````

**Réponse** : 
*Ligne 3* : Il initialise la variable résultat à la valeur du dernier élement du tableau au carré . 
*Ligne 4* : Il change la valeur de la variable résultat par la division de la valeur précédente de résultat par le quatrième élément du tableau. 
*Ligne 5* : On affiche résultat
**Le code retournera le chiffre 10 .** 

3️⃣ De quel facon peut-on **simplifier** le **code** suivant ?
````
a = 5 ; b = 3 ; c = a \* b
a = b + a 
c = c / b
b = a \* c 
print ( b )
````

**Réponse** : 
````
a = 5 ; b = 3 ; c = a \* b
a += b  
c /= b
b = a \* c 
print ( b )
````

4️⃣ Que fait le **code suivant** ? **Modifier** le pour qu'il soit plus **explicite**
````
a = 0.5
b = int( input ( "Veuillez insérer un chiffre :" ) )
print ( b * a )
````

**Réponse** : 
Il permet de diviser un chiffre entier par deux.
````
b = int( input ( "Veuillez insérer un chiffre à diviser par 2 :" ) )
print ( b \ 2 )
````

5️⃣ **Compléter** ce code
````
# Ce programme permet de retourner l'aire d'une figure rectangulaire droite grâce à sa longueur et sa largeur 
# On commence par demander la longueur 
longueur = input( "Veuillez indiquer la longueur de la forme en mm : ")
# Puis on demande la largueur 
largueur = input( "Veuillez indiquer la largueur de la forme en mm : ")
# On calcule l'aire avec la formule **longueur x largueur** 
aire = int(longueur) * int(largueur)
# On termine par afficher l'aire de la figure 
print(f" L'aire de la figure rectangulaire est égale à { aire }" )	
````
----
### 🏗 Partie application 🏗

Ecrire un **programme** permettant de calculer l'**aire** d'un **triangle quelconque** avec pour valeur d'entrée sa **hauteur** et sa **base**

⭐ **Bonus** ⭐ Ecrire un **programme** permettant de calculer l'**hypothénuse** d'un triangle **quelconque** à partir de **pythagore** 

____
### 🧠Ce qu'il faut retenir 🧠
 - Toujours assigner une valeur à une variable avant de l'utiliser
 - Une variable peut avoir plusieurs types :  int ( chiffre entier ) , float ( chiffre décimal ) , bool ( true / false) , array ( tableau de valeur ), str ( chaine de caractère ), 
 - Une variable qui ne va pas changer durant tout le long d'un programme est appelé : une constante ( tels que pi )
 - Le nom d'une constante s'écrira uniquement en majuscule ( ex : ``PI`` ) alors qu'une variable s'écrit uniquement en minuscule ( ex : ``age``  , ``birth_date`` ) cela permet de rapidement faire la différence.
- Un tableau commence toujours à la position 0 , pour récupérer la valeur dans le tableau à une position donné on utilise les crochets [ ] ( ex : ``tableau[4]`` -> nous récupérons donc le 5ème élément du tableau )
- La fonction input retourne une valeur de type str , si on demande à l'utilisateur de renter un nombre il faut donc utiliser la fonction ``int( )`` pour le convertir en type int .
- La fonction`` print( )`` permet d'afficher un texte dans la console , on ne peut afficher qu'un type de variable à la fois sauf dans le cas d'interpolation en utilisant le symbole ``f`` et en encadrant les interpolations par des accolades.( ex : ``print( f" Vous avez { age } ans ")`` )
- Toujours être très explicite dans ce qu'on demande à l'utilisateur et dans ce qu'on lui montre 