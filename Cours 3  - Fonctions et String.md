----
### ⌛Questions cours précédents ⌛

1️⃣  Quels sont les **deux types** de **boucles** possibles ? et comment les **utiliser** ?

2️⃣  Comment **vérifier** si une **valeur** fait **partie** d'une **tableau** de valeur ou d'une **chaine** de caractère ? 

3️⃣   Comment faire une **boucle infini** ?

-----
### ☑️Partie QCM ☑️

1️⃣  Quelles sont les **éléments** nécessaire à la **construction** d'une **fonction** ?
- [ ] un nom
- [ ] un ou des paramètres
- [ ] un return
- [ ] un bloc d'instruction

2️⃣  Quelle **synthaxe** de **fonction** est **incorrecte**  ?
- [ ] def fonction1( a ,b ):
- [ ] def fonction_deux( ):
- [ ] def fonctionTrois( ):
- [ ] def fonction-quatre( a,b,c,d,e,f,g,h,i,j):

3️⃣  Combien de **paramètre** peux avoir une **fonction** ?
- [ ] 0
- [ ] au moins 1
- [ ] pas de limite
- [ ] au maximum 99

4️⃣  Que permet le **return** dans une **fonction**?
- [ ] Sortir d'une fonction
- [ ] Retourner à la ligne
- [ ] Renvoyer une valeur en sortie de fonction
- [ ] Relancer la fonction

5️⃣  Quel **synthaxe** permet d'**attribuer** une valeur à un paramètre par **défaut** dans une **fonction**?
- [ ] def fonction5( a = 10 ) :
- [ ] def fonction6( b : 10) :
- [ ] def fonction7( c -> 10) :
- [ ] def fonction8( d => 10) :

6️⃣  Quels **fonctions** permet de **transformer** n'importe quel type de variable en **string** ?
- [ ] str()
- [ ] repr()
- [ ] string()
- [ ] toString()

7️⃣  Parmis les **fonction suivantes**, lesquelles sont **utilisables** sur une **chaine de caractère**?
- [ ] upper()
- [ ] count()
- [ ] replace()
- [ ] slice()

8️⃣  Que se passe t-il en **executant** le **code suivant** : `print(("pomme" * 2) + "dapi")`?
- [ ] Le code ne fonctione pas
- [ ] On affiche "pomme pomme dapi"
- [ ] On affiche "pomme2dapi"
- [ ] On affiche "pommepommedapi"

9️⃣  Quel **syntaxe** permet de **rechercher** la **première occurence** d'un **mot** dans une **chaine de caratère** ?
- [ ] chaine.index(  "mot " )
- [ ] chaine.find( "mot")
- [ ] chaine.rfind( "mot" )
- [ ] chaine.first( "mot" )

🔟 Quelle **fonction** permet de retourner la **longueur** d'une **string** ou d'un **tableau** ? 
- [ ] length( )
- [ ] len( )
- [ ] size( )
- [ ] long( )

----
### 📝 Partie correction pratique 📝

1️⃣ Ce **code** va t'il **correctement** s'**éxécuter** ? Pourquoi ?
````
message = "Hello world !"

def display_message(message):

	print(message)

display_message()
````

2️⃣ Que retourne l'**éxécution** de ce **code** ? 
````
import random

def randomID():

    id = ""

    while len(id) < 10:

        id += str(random.randint(0,9))

    return id  

print( randomID() )

````

3️⃣ De quel facon peut-on **simplifier** le **code** suivant ?
````
mot=" "

while " " in mot:

    mot = input("Veuillez insérer un mot sans espace ! :")

    longueur = 0

    for i in mot:

        longueur+=1

print(f"Votre mot fait {longueur} lettres")
````

4️⃣ Que permet le **code** suivant ? **Modifier** le pour qu'il soit plus **explicite**
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

5️⃣ **Compléter** ce code
````
# Programme pour censurer les gros mots dans une phrase entré par l'utilisateur

# On initialise une constance tableau des gros mots à censurer

........ = [ "merde" , "putain" , "connard" ]

# On demande une phrase à l'utilisateur 

phrase = .......("Veuillez insérer une phrase à corriger :")

# On attribue la valeur de la phrase à la phrase censuré dans un premier temps

censored_phrase = .....

# On crée la fonction qui permet de générer une censure avec la même longueur que le mot donné en paramètre

def censored_bad_word(....):

    return "*" * len(.....)

# On itère sur chaque gros mot du tableau gros mots et on vérifie si il se trouve dans la phrase si c'est le cas on remplace le mot par la censure généré grâce à la fonction précédente. 

for bad_word in BAD_WORDS :

    if .... in censored_phrase :

        censored_phrase = ..........replace( ..... , censored_bad_word(......) )

# On affiche la phrase avec les censures appliqués 

print( f"Voici votre phrase corrigé : \"{........}\" " )

## Fin du programme ##

````

----
### 🏗 Partie application 🏗

Ecrire un **programme** pour **convertir** une **température** depuis n'importe quel **unité** vers n'importe quel **unité**

⭐ Bonus ⭐