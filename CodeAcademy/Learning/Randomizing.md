# Randomizing

This section introduces Randomizing into Go. This generates random number and uncertainties within Go, using `math/rand` in the import library we are able to 
generate a random integer.

```go
import (
  "math/rand"
   "fmt"
)

func main() {
  fmt.Println(rand.Intn(100))
}
```
With the `rand` as a random number, this specific `fmt` will print out integers from `0` to `99`

## Challenge

1. Use `rand.Intn()` to generate a new random integer for `amountLeft`. Use an argment of `10000` so the max possible value generated is `9999`.

## My Code

```go
package main

import (
	"fmt"
  "math/rand"
)

func main() {
	// Edit amountLeft below: 
  amountLeft := 10000
  
  fmt.Println("amountLeft is: ", (rand.Intn(amountLeft)))
  
	if amountLeft > 5000 {
		fmt.Println("What should I spend this on?")
  } else {
    fmt.Println("Where did all my money go?")
  }
}
```
Unfortunately this solution was incorrect. It's incorrect at `fmt.Println("amountLeft is: ", (rand,Intn(amountLeft)))` . 

## Correct solution
```go
package main

import (
	"fmt"
  "math/rand"
)

func main() {
	// Edit amountLeft below: 
  amountLeft := rand.Intn(10000)
  
  fmt.Println("amountLeft is: ", amountLeft)
  
	if amountLeft > 5000 {
		fmt.Println("What should I spend this on?")
  } else {
    fmt.Println("Where did all my money go?")
  }
}
```
