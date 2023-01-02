-----
### ☑️Partie QCM ☑️

1️⃣ Comment **peut-on décrire** une **variable** ?
- [ ] Un conteneur stockant une valeur fixe 
- [ ] Un conteneur dont la valeur peut être modifé
- [ ] Elle peut avoir plusieurs type de valeur simultanément 
- [ ] Il est obligatoire de lui attribuer une valeur avant d'effectuer des opérations avec celle-ci

2️⃣ Lesquels de ces **types** peut être **attribué** à une **variable** ?
- [ ] int 
- [ ] float 
- [ ] string
- [ ] bool 

3️⃣ Quel **fonction** utiliser pour convertir **"0"** en **0**  ?
- [ ] int()
- [ ] string()
- [ ] number()
- [ ] integer()

4️⃣ Lequel de ces **opérateurs** n'est pas un **opérateur arithmétique** ?
- [ ] +
- [ ] **
- [ ] =
- [ ] %

5️⃣ Quel **opérateur** utilisé pour avoir le **reste** qu'une **division** entre **a** et **b** ?
- [ ] a/b
- [ ] a%b
- [ ] a//b
- [ ] a\*b

6️⃣ Quel **opérateur** permet d'attribuer à **c** le résultat de la **puissance** de **c** par **x**  ?
 - [ ] c += x
 - [ ] c %= x
 - [ ] c \*\*= x
 - [ ] c \*= x

7️⃣ Quel **fonction** utilisé pour afficher la variable **a** ?
- [ ] show(a)
- [ ] display(a) 
- [ ] input(a)
- [ ] print(a)

8️⃣ Comment demander une variable **b** à l'utilisateur ?
- [ ] b = input("Indiquer b :")
- [ ] b = give("Indiquer b :")
- [ ] b = send("Indiquer b :")
- [ ] b = indicate("Indiquer b :")

9️⃣ Comment créer un **tableau de valeurs** ?
- [ ] tableau = 1 2 3 4
- [ ] tableau = [ 1 , 2 , 3 , 4 ]
- [ ] tableau = [ 1 2 3 4 ]
- [ ] tableau = { 1 : 2 : 3 :4 }

🔟 Comment récupérer le **dernier élément** du **tableau** précédént  ? 
- [ ] tableau[0]
- [ ] tableau[1]
- [ ] tableau[-1]
- [ ] tableau[x]

----
### 📝 Partie correction pratique 📝

1️⃣ Ce code va t'il **correctement** **s'éxécuté** ? Si non **pourquoi** ?
````
b = 0
b = a
print ( a )
````
2️⃣ Que retourne l'**éxécution** de ce **code** ? 
````
a = 0 ; b = 3 ; c = 4 ; d = 10
tableau = [ a , b , c , d ]
résultat = tableau [ -1 ] \*\*2
résultat /= tableau [ b ]
print( résultat )
````
3️⃣ De quel facon peut-on **simplifier** le **code** suivant ?
````
a = 5 ; b = 3 ; c = a \* b
a = b + a 
c = c / b
b = a \* c 
print ( b )
````
4️⃣ Que fait le **code suivant** ? **Modifier** le pour qu'il soit plus **explicite**
````
a = 0.5
b = int( input ( "Veuillez insérer un chiffre :" ) )
print ( b \* a )
````
5️⃣ **Compléter** ce code
````
# Ce programme permet de retourner l'aire d'une figure rectangulaire droite grâce à sa longueur et sa largeur 
# On commence par demander la longueur 
............ = input( "Veuillez indiquer la ............. de la forme")
# Puis on demande la largueur 
............ = input( "Veuillez indiquer la ............. de la forme")
# On calcule l'aire avec la formule **longueur x largueur** 
aire = ........ \* ............
# On termine par afficher l'aire de la figure 
.........(f " L'aire de la figure rectangulaire est égale à { aire }" )	
````
----
### 🏗 Partie application 🏗

Ecrire un **programme** permettant de calculer l'**aire** d'un **triangle quelconque** avec pour valeur d'entrée sa **hauteur** et sa **base**

⭐ **Bonus** ⭐ Ecrire un **programme** permettant de calculer l'**aire** d'un triangle **quelconque** à partir de **pythagore** 
