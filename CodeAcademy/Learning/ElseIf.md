# Else if Statement

Adding `else if` to `if..else` statments allows us to check another condition after `if` statement checks its condition. There are infinite amounts of `else if` statments
that can be added.

The `else if` statement will always come after an `if` statement. if we have an `else` statement, then `else if` comes before.

### Syntax

```go
position := 2

if position == 1 {
  fmt.Println("You won the gold!")
 } else if position == 2 {
  fmt.Println("You got the silver medal.")
 } else if position == 3 {
  fmt.Println("Great Job on Bronze!")
 } else {
  fmt.Println("Sorry, try again next year")
 }
 ```
### Challenge

Add an `else if` statement that checks if `amountStolen` is greater than or equal to `5000` to the existing `if...else` statement.
If the condition evaluates to true, print the string `"Thhink of all the candy we can buy!"

### Accepted Code

```go
package main

import "fmt"

func main() {

amountStolen := 64650

if amountStolen > 1000000 {
	fmt.Println("We've hit the jackpot!")
} else if amountStolen >= 5000 {
		fmt.Println("Why did we even do this?")
} else {
    fmt.Println("Think of all the candy we can buy!")
}
}
```
