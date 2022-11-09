# Seeding

One way to get a unique number everytime we roll our code is to use `time`. The reason why we use `time` is because its always a different time the 
program runs.

**For example**
```go
package main

import (
  "fmt"
  "math"
  "time"
)
 
func main() {
  rand.Seed(time.Now().UnixNano())
  fmt.Println(rand.Intn(100))
}
```
Doing this we import the `time` library, call the `.Now()` along side with `.UnixNano()` method. The number we get from `time.Now().UnixNano()` inside 
our `rand.Seed()` will result in a different seed value each time. Now we just need to set parameters of a variable in order for it to run.

## Challenge
```go
package main

import (
  "fmt"
  "math/rand"
  "time"
)

func main() {
	// Add your code below:
  rand.Seed(time.Now().UnixNano())
  
  amountLeft := rand.Intn(10000)
  
  fmt.Println("amountLeft is: ", amountLeft)
  
	if amountLeft > 5000 {
		fmt.Println("What should I spend this on?")
  } else {
    fmt.Println("Where did all my money go?")
  }
}
```
Whenever you run this, the `amountLeft` will always be randomized, and the `fmt.Println` will act accordingly to the result
