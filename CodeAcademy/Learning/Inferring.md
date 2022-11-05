# Inferring
<p> There is a way to declare a variable without explicitly stating its type using the declaration := operator. 
  This powerful operator may be utilized in many different ways for instance : </p>
 
  ```go
  vienIsHungry := 7/10
  iAmSleepy := false
  gymTimeBro := "I am Spain without the S"
  ```
 Above we declared different times of declarations; a bool, a float, and a string by using :=.
 </br>
 Go also utilizes var 
 
   ```go
  var vienIsHungry = 7/10
  var iAmSleepy = false
  var gymTimeBro := "I am Spain without the S"
  ```
  
  This solution is equally the same and effective, however it may take longer. 
 </br>
 
 This is a problem that I worked on utilizing the := operator. 
  
```go
package main

import "fmt"

func main() {
  // Define daysOnVacation using := below:
  daysOnVacation := 7
  
  // Define hoursInDay using var and = below:
  var hoursInDay  = 24
  
  fmt.Println("You have spent", daysOnVacation * hoursInDay, "hours on vacation.")
}
```

Solution = You have spent 168 hours on vacation.
