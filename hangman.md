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
Implement a function that can convert a `String` to a `List Letter`:
```elm
createLetters : String -> List Letter
```
Change the `contains` function to fit the following signature:
```elm
contains : List Letter -> Char -> Bool
```
Implement a function that reveal the `Letter` if the input `Char` is correct.
```elm
revealSingle : Char -> Letter -> Letter
```
Using `List.map` and `revealSingle`, implement a function that reveal all letters corresponding to a given input `Char`.
```elm
reveal : Char -> List Letter -> List Letter
```

```elm
foo : Char -> List Letter -> Int -> Int
```
Our futur program will contain a `Model` type that will hold the word to guess, and a counter reprensenting the number of tries left. Here is a possible implementation:
```elm
type alias Model =
    { letters : List Letter
    , counter : Int
    }
```
Here is a syntax example of updating a `v0` of type `Vector` record:
```elm
{ v0 | x = v0.x + 1 }
```
Implement the function that will update the `Model` with a given input `Char`:
```elm
handle : Char -> Model -> Model
```