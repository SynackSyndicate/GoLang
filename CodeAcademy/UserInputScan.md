# Utilizing Go to obtain User Input!

.Scan() which allows us to get End-User Input. 

For Example
```go
 fmt.Println("How are you doing?")

  var response string

 fmt.Scan(&response)

 fmt.Printf("I'm %v", response)
```

Which prints out into bash
```go
"How are you doing?"
// User Inputs
"Good"
// Returns 
"I'm Good"
```
However, if a user puts "Not Bad" it returns "I'm Not." That is because only 1 %v was saved and the code isn't allowing for any more clauses.
</br> 
</br>
To mitigate this
```go
fmt.Println("How are you doing?")

var response1 string
var respnse2 string
fmt.Scan(&response1)
fmt.SCan(&response2)

fmt.Printf("I'm %v %v", response1, response2)
```

### My Challenge
1. Declare `string` variable named `food`
2. Call `fmt.Scan()` with the argument `&food`
3. Enter command `go run main.go`

```go
package main

import "fmt"

func main() {
  fmt.Println("What would you like for lunch?")
  
  // Add your code below:
  var food string
  
  fmt.Scan(&food)
  
  fmt.Printf("Sure, we can have %v for lunch.", food)
}
```
