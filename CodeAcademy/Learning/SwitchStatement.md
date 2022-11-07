# Switch Statement

`else if` statements are good for multiple conditions, but looking over too many can be overwhelming.

```go
vienEats := "ramen"

if vienEats == "pho" {
  fmt.Println("Would you want Small, Medium, Large bowl?"
  } else if == "Korean BBQ" {
  fmt.Println("It'll cost $45 per person for the dinner price.")
  } else if == "ramen" {
  fmt.Println("Spicy or Regular?")
  }
 ```
 
 Coding this would be very tedious and daunting to read. Instead Go uses `switch` to use alternative syntaxes
 
 ```go
 vienEats := "ramen"
 
 switch vienEats {
 case "pho":
  fmt.Println("Would you want Small, Medium, Large bowl?")
 case "Korean BBQ"
  fmt.Println("It'll cost $45 per person for the dinner price.")
 case "ramen"
  fmt.Println("Spicy or Regular?")
 default
  fmt.Println("I'm not hungry")
 }
```
These types of codes execute the same objective, however the `switch` statement makes it easier to read, code, and compartmentalize. `Else if` is a lot of 
logic and tedious to work with. Notice `default` is included here. `default` is used here if none of the `case` choices has been selected.
