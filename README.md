## terminal

`ls` -  liste les fichiers du dossier courant
`ls -a`- liste les fichiers du dossier courant en affichant les fichiers cachés
`cd [directory]` - naviguer vers le dossier
`..` - dossier parent
`.` - dossier courant
`/` - dossier racine
`code [file name / directory]` - ouvrir le fichier / dossier dans VSCode
`mkdir [directory name]` - créer un dossier
`touch [file name]` - créer un fichier
`rm [file name]` - supprimer un fichier
`cat [file name]` - afficher le contenu d'un fichier
`open [file name]` - ouvrir le fichier avec l'application prévue par défaut
 
## git

Système de versioning de code.

`git status` - connaître l'état de git
`git add [fichier]` - ajouter un fichier au prochain commit
`git add .` - ajouter l'ensemble des modifications au prochain commit
`git commit -m "message"` - écrire un commit
`git push` - envoyer le code vers le repository distant
`git pull` - récupérer le code distant

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

## Divers

`elm make [file name]` - compiler un fichier Elm
`python3 [file name]` - exécuter un script python