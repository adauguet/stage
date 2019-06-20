# Hangman project

Implement de following function:
```elm
contains : String -> Char -> Bool
```
Create a type `Letter` that contains a `Char` and a `Bool` to keep track if the letter is revealed or not. Here is an example of a custom type:
```elm
type alias Vector =
    { x : Float
    , y : Float
    }
```
Implement the following function:
```elm
createLetters : String -> List Letter
```
Change the `contains` function to fit the following signature:
```elm
contains : List Letter -> Char -> Bool
```
We are going to introduce the concept of a counter.
