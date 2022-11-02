# Sprintf Method

Interpolating a string, without **printing** it, we can use fmt.Sprintf(). Just like fmt.PrintF(), fmtSprintf() can use verbs.
</br>
</br>
For example:
```
correctAns := "V was here"
whoWasHere := fmt.Springf("What does this graffiti say? %v", whoWasHere)

fmt.Print(whoWasHere) // Prints: What does this graffiti say? V was here.
```
## Exercise

Assign to wish the value of calling fmt.Sprintf() with the values template and pet.

wish should then contain the interpolated string "I wish I had a puppy.".

```
package main

import "fmt"

func main() {
  template := "I wish I had a %v."
  pet := "puppy"
  
  var wish string
  
  // Add your code below:
  wish = fmt.Sprintf(template, pet)
  
  fmt.Println(wish)
  // Prints: I wish I had a puppy.
}
```
