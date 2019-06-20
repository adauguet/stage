# Hangman project

## Contains

Using `String.toList` and `List.member`, implement a function that checks if a `String` contains a given `Char`:
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
And here is the beginning of `Letter`:
```elm
type alias Letter =
    { -- write properties here
    }
```

We are going to need a few convenience functions:
- implement a function that can create a `Letter` from a `Char`:
    ```elm
    fromChar : Char -> Letter
    ```
- reciprocally, implement the function that converts a `Letter` to a `Char`:
    ```elm
    toChar : Letter -> Char
    ```

Change the `contains` function to fit the following signature:
```elm
contains : List Letter -> Char -> Bool
```

## Initialisation

Using `List.map` and `fromChar`, implement a function that can convert a `String` to a `List Letter`:
```elm
createLetters : String -> List Letter
```

## Reveal letters

Using `if ... then ... else`, implement a function that updates a `Letter` if the input `Char` equals the one contained in the `Letter`.
```elm
revealLetter : Char -> Letter -> Letter
```

Using `List.map` and `revealSingle`, implement a function that reveals all letters corresponding to a given input `Char`.
```elm
revealLetters : Char -> List Letter -> List Letter
```

## Counter

Our program will use a counter to track the number of tries left. Using `if ... then ... else`, implement a function that will decrement a counter if the input `Char` is not contained in the list of letters: 
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