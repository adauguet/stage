## terminal

- `ls` -  liste les fichiers du dossier courant
- `ls -a`- liste les fichiers du dossier courant en affichant les fichiers cachés
- `cd [directory]` - naviguer vers le dossier `..` - dossier parent
- `.` - dossier courant
- `/` - dossier racine
- `code [file name / directory]` - ouvrir le fichier / dossier dans VSCode
- `mkdir [directory name]` - créer un dossier
- `touch [file name]` - créer un fichier
- `rm [file name]` - supprimer un fichier
- `cat [file name]` - afficher le contenu d'un fichier
- `open [file name]` - ouvrir le fichier avec l'application prévue par défaut
 
## git

Système de versioning de code.

- `git status` - connaître l'état de git
- `git add [fichier]` - ajouter un fichier au prochain commit
- `git add .` - ajouter l'ensemble des modifications au prochain commit
- `git commit -m "message"` - écrire un commit
- `git push` - envoyer le code vers le repository distant
- `git pull` - récupérer le code distant

github.com - permet d'héberger des repository sur internet.

## principaux langages

##### Web (front-end)
HTML + CSS + Javascript
React.js / Angular.js
(Elm)

##### back-end
Go / Node.js ...

##### Mobile
Swift (iOS), Kotlin/Java (Android)

##### Logiciels
C, C++, Java

##### Scripts
Python

##### Base de données
SQL

##### Autres
Haskell

Certains languages sont compilés, c'est à dire traduis en instructions bas niveau par un **compilateur**. Intérêts :
- optimisation du code et donc des performances
- vérification du code et détection d'erreurs

Dans un language, on manipule des **types**, des **valeurs**, des **fonctions**.
- `String` est un type qui représente une chaîne de caractères
- `"Hello world!"` est une valeur de type `String`
- `sayHello : Int -> String` est une fonction qui s'appelle `sayHello`, qui prend en paramètre un `Int` et renvoie une `String`.
## Requêtes HTTP

Protocole de communication entre deux services. Chaque requête reçoit une réponse.

- méthode : `GET`, `POST` en fonction du sens de la requête
- url : adresse, peut contenir des paramètres `https://www.google.com/chemin?clé=valeur`
- code d'erreur (réponse): `200`, `404`, `500`...

JSON - format de données utilisé pour structurer des données, notamment dans le contenu des requêtes HTTP

## Elm

Exemple de programme
```
module Main exposing (helloWorld, helloName)

helloWorld : String
helloWorld =
    "Hello world!"

helloName : String -> String
helloName name =
    "Hello " ++ name ++ "!"
```
- la fonction `helloWorld` ne prend pas de paramètre et renvoie une valeur de type `String`
- la fonction `helloName` prend un paramètre `name` de type `String` et renvoie une valeur de type `String`


### Elm make

- `elm make [fichier Elm]` : compile un fichier Elm

### Elm REPL

Pour ouvrir Elm REPL, deux possibilités :
- entrer `elm repl` dans un terminal
- utiliser la commande incluse dans VSCode : *View > Command Palette* puis chercher "Elm REPL"

Elm REPL permet d'exécuter du code Elm. En reprenant le code précédent :
- `import Main` : importe le module `Main`, on peut ensuite appeler la fonction `Main.helloWorld` ou `Main.helloName "Julien"`.
- `import Main exposing (helloWorld, helloName)` : importe le module `Main` en exposant les fonctions `helloWorld` et `helloName`. On peut ensuite appeler la fonction `helloWorld` ou `helloName "Paul"`.

- `:exit` : quitter Elm REPL


## Exercices

Implémenter les fonctions suivantes :
```
add : Int -> Int -> Int
```
```
multiply : Float -> Float -> Float
```

Dans le cas d'un polynôme de degré 2, implémenter la fonction suivante :
```
discriminant : Float -> Float -> Float -> Float
```
En utilisant la fonction `discriminant`, implémenter la fonction `nombreRacines` qui renvoie `0`, `1` ou `2`, le nombre de racines du polynôme de degré 2. Indice : il faut utiliser une condition `if ... then .. else`.
```
nombreRacines : Float -> Float -> Float -> Int
```
En modifiant la fonction précédente, implémenter la fonction `resolve` qui résoud les polynômes de degré 2. On utilise une `List` pour renvoyer la liste des racines. Exemple : `[a, b]`.
```
resolve : Float -> Float -> Float -> List Float
```

Implémenter la fonction suivante :

```
computeKnightMovements : (Int, Int) -> List (Int, Int)
```

## Divers

- `python3 [file name]` - exécuter un script python

### npm

NPM est un gestionnaire de packages disponible sous linux et macos.

#### Installation

npm est inclus dans l'installation de Node.js. Pour installer Node.js, suivre les instructions à l'adresse suivante : https://nodejs.org/en/

#### Utilisation

- `npm install -g elm` : install Elm de manière globale (pour tous les utilisateurs)