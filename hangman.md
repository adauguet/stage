# Hangman project

## Contains

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
Implement a function that can convert a `String` to a `List Letter`:
```elm
createLetters : String -> List Letter
```
Change the `contains` function to fit the following signature:
```elm
contains : List Letter -> Char -> Bool
```

## Reveal letters

Implement a function that reveal the `Letter` if the input `Char` is correct.
```elm
revealLetter : Char -> Letter -> Letter
```
Using `List.map` and `revealSingle`, implement a function that reveal all letters corresponding to a given input `Char`.
```elm
revealLetters : Char -> List Letter -> List Letter
```

## Counter

Our program will use a counter to track the number of tries left. Implement a function that will decrement a counter if the input `Char` is not contained in the list of letters: 
```elm
updateCounter : Char -> List Letter -> Int -> Int
```

## Model

We will use a type `Model` to hold the letters to guess and the counter. Write a `Model` type with both properties.
```elm
type alias Model =
    { -- write properties here
    }
```
Using `reveal` and `updateCounter`, implement the function that will update the `Model` accordingly with a given input `Char`:
```elm
updateModel : Char -> Model -> Model
```