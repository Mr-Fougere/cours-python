----
### ⌛Questions cours précédents ⌛

1️⃣  Quels sont les deux types de boucles possibles ? et comment les utiliser ?

**Réponse :**
La boucle while et la boucle for 
``while **condition** :``
``for **i** in **tableau de valeur** :``
La boucle while a seulement besoin d'une condition.
La boucle for a besoin d'une variable d'itération et d'un tableau de valeur.

2️⃣  Comment vérifier si une valeur fait partie d'une tableau de valeur ou d'une chaine de caractère ? 

**Réponse :** 
On utilise l'opérateur d'appartenance ``in`` 
``valeur in tableau ``
valeur in chaine

3️⃣   Comment faire une boucle infini ?

Réponse:
``While 1:``

-----
### ☑️Partie QCM ☑️

1️⃣  Quelles sont les éléments nécessaire à la construction d'une fonction ?
- [x] un nom
- [ ] un ou des paramètres
- [ ] un return
- [x] un bloc d'instruction

2️⃣  Quelle synthaxe de fonction est incorrecte  ?
- [ ] def fonction1( a ,b ):
- [ ] def fonction_deux( ):
- [ ] def fonctionTrois( ):
- [x] def fonction-quatre( a,b,c,d,e,f,g,h,i,j):

3️⃣  Combien de paramètre peux avoir une fonction ?
- [x] 0
- [ ] au moins 1
- [x] pas de limite
- [ ] au maximum 99

4️⃣  Que permet la fonction return dans une fonction?
- [x] Sortir d'une fonction
- [ ] Retourner à la ligne
- [x] Renvoyer une valeur en sortie de fonction
- [ ] Relancer la fonction

5️⃣  Quel synthaxe permet d'attribuer une valeur à un paramètre par défaut dans une fonction?
- [x] def fonction5( a = 10 ) :
- [ ] def fonction6( b : 10) :
- [ ] def fonction7( c -> 10) :
- [ ] def fonction8( d => 10) :

6️⃣  Quels fonctions permet de transformer n'importe quel type de variable en string ?
- [x] str()
- [x] repr()
- [ ] string()
- [ ] toString()

7️⃣  Parmis les fonction suivante, lesquelles son utilisable sur une chaine de caractère?
- [x] upper()
- [x] count()
- [x] replace()
- [ ] slice()

8️⃣  Que se passe t-il en executant le code suivant : `print(("pomme" * 2) + "dapi")`?
- [ ] Le code ne fonctione pas
- [ ] On affiche "pomme pomme dapi"
- [ ] On affiche "pomme2dapi"
- [x] On affiche "pommepommedapi"

9️⃣  Quel syntaxe permet de rechercher la première occurence d'un mot dans une chaine de caratère ?
- [ ] chaine.index(  "mot " ) 
- [x] chaine.find( "mot")  => permet de retrouver la 1er occurence dans une chaine
- [ ] chaine.rfind( "mot" ) 
- [ ] chaine.first( "mot" ) 

🔟 Quel fonction permet de retourner la longueur d'une string ou d'un tableau ? 
- [ ] length( )
- [x] len( )
- [ ] size( )
- [ ] long( )

----
### 📝 Partie correction pratique 📝

1️⃣ Ce code va t'il correctement s'éxécuter ? Pourquoi ?
````
message = "Hello world !"

def display_message(message):

	print(message)

display_message()
````

**Réponse :**
Le code va renconter une erreur car la fonction display_message( ) n'a pas recu de paramètre pour s'effectuer correctement. La variable message dans la fonction display_message n'est pas la même que la variable message initialiser au début du script. Il s'agit d'une variable de fonction et d'une variable global. 

2️⃣ Que retourne l'éxécution de ce code ? 
````
import random

def randomID():

    id = ""

    while len(id) < 10:

        id += str(random.randint(0,9))

    return id  

print( randomID() )

````

**Réponse :**
Le code retourne un ID composé de 10 chiffres aléatoires.

3️⃣ De quel facon peut-on simplifier le code suivant ?
````
mot=" "

while " " in mot:

    mot = input("Veuillez insérer un mot sans espace ! :")

    longueur = 0

    for i in mot:

        longueur += 1

print(f"Votre mot fait {longueur} lettres")
````

**Réponse :**

On peut tout simplement utiliser la fonction len qui retourne le nombre de caractere dans une chaine de caractère.
````
mot=" "

while " " in mot:

    mot = input("Veuillez insérer un mot sans espace ! :")

longueur = len(mot)

print(f"Votre mot fait {longueur} lettres")
````

4️⃣ Que permet le code suivant ? Modifier le pour qu'il soit plus explicite
````
word=" "

def fonction1(word):
	
	out = ""
	
	for i in word:
		
		out = i + out
	
	return out

while " " in mot:

	flag = False
    
    word = input("Veuillez insérer un mot sans espace ! :")
	
	word2 = fonction1(word)
	
	if mot == mot2:
	
	   flag = True

print(flag)
````

**Réponse :**
Le code suivant permet de savoir si le mot est un palindrome.
La fonction 1 permet d'inverser le sens des lettres d'un mot, on peut donc la renommer ``reverse_string``. 
La variable ``flag`` correspond à la réponse : " Le mot est-il un palindrome ?", on peut donc la renommer ``isPalindrome``.
L'input n'est pas très explicite, on notifie à l'utilisateur que l'on recherche si le mot est un palindrome.
Le print de fin également néccesite d'être plus explicite pour notifier à l'utilisateur que son mot est un palindrome.

````
word=" "

def revers_string(word):
	
	reversed_string = ""
	
	for i in word:
		
		reversed_string = i + reversed_string
	
	return reversed_string

while " " in word :

	isPalindrome = False
    
    word = input("Veuillez insérer un mot sans espace ! :")
	
	reversed_word = reverse_string(word)
	
	if word == reversed_word :
	
	   isPalindrome = True

if isPalindrome:

	print(f" Le mot {word} est un palindrome.")

else :

	print(f" Le mot {word} n'est pas un palindrome.")

````

5️⃣ Compléter ce code
````
# Programme pour censurer les gros mots dans une phrase entré par l'utilisateur

# On initialise une constance tableau des gros mots à censurer

BAD_WORDS = [ "merde" , "putain" , "connard" ]

# On demande une phrase à l'utilisateur 

phrase = input("Veuillez insérer une phrase à corriger :")

# On attribue la valeur de la phrase à la phrase censuré dans un premier temps

censored_phrase = phrase

# On crée la fonction qui permet de générer une censure avec la même longueur que le mot donné en paramètre

def censored_bad_word(word):

    return "*" * len(word)

# On itère sur chaque gros mot du tableau gros mots et on vérifie si il se trouve dans la phrase si c'est le cas on remplace le mot par la censure généré grâce à la fonction précédente. 

for bad_word in BAD_WORDS :

    if bad_word in censored_phrase :

        censored_phrase = censored_phrase.replace( bad_word , censored_bad_word(bad_word) )

# On affiche la phrase avec les censures appliqués 

print( f"Voici votre phrase corrigé : \"{censored_phrase}\" " )

## Fin du programme ##

````

----
### 🏗 Partie application 🏗

Ecrire un **programme** pour **convertir** une **température** depuis n'importe quel **unité** vers n'importe quel **unité**

⭐ Bonus ⭐

Ecrire un programme pour générer du texte aléatoire ( s'inspirer de lorem ipsum )

---
### 🧠Ce qu'il faut retenir 🧠

- Une fonction doit obligatoiremtn avoir un nom ( sans tiret - ) et un bloc d'instruction.
- Une fonction peut avoir 0 ou plusieurs paramètres, si une valeur par défaut n'est pas défini pour un paramètre il faut obligatoirement le renseigner pour le bon fonctionnement de celle-ci.
- Les paramètres d'une fonction , sont considérés comme des variables locales à celle-ci , utilisable uniquement au sein d'ELLE ! 
- On peut uniquement appeler une fonction après l'avoir déclaré .
- Dans le cas, ou l'on veux retourner une valeur à la fin d'une fonction on utilise la fonction return qui sortira de la fonction et retournera la valeur qui la suite ( si aucune valeur ne la suite alors il retournera None )
- Il est évidemment possible d'imbriquer des fonctions l'une dans l'autre. 
- Fonctions pour chaine de caractère à retenir 
	- [ ] **find( )** => retourne la première occurence en partant du début de la valeur donné en paramètre
	- [ ] **replace( )** => remplace toutes les valeurs donnée en premier paramètre par le deuxième paramètre
	- [ ] **len( )** => retourne sa longueur en int 
	- [ ] **upper( )** => transforme tous les caractères en majuscule
	- [ ] **lower( )** => transforme tous les caractères en minuscule 
	- [ ] **count( )** => retourne le nombre d'occurence de la valeur entré en paramètre en int 
- Fonctions pour tableau de valeur à retenir 
	- [ ] **len( )** => retourner sa longueur en int 
	- [ ] **index( )** => retourne la place de la première occurence du paramètre donné
	- [ ] **pop( )** => supprime la dernière valeur si aucun paramètre n'est donné sinon supprime la valeur à la position donnée
	- [ ] **remove( )** => supprime la première occurence trouvé correspondant à la valeur du paramètre
	- [ ] **count( )** => retourne le nombre d'occurence de la valeur entré en paramètre en int
