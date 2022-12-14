# Comic Mischief Project
<p>
Part of Codeacademy learning is implementing half way point project on what we learned so far. At this point in my journey of GoLang, 
I've learned how to create a main.go file, create a package main, import "fmt", determine func main (){ [insert declarations here],
and finalize the code with fmt.Println(). This project, Comic Mischief, incorporates those fundamental skills.
  </p>

## The Code
```go
package main

import "fmt"

func main () {
  
var publisher, writer, artist, title string

title = "Mr. GoToSleep"
writer = "Tracy Hatchet"
artist = "Jewel Tampson"
publisher = "DizzyBooks Publishing Inc."

var year uint 
var pageNumber uint

year = 1997
pageNumber = 14

var grade float32

grade = 6.5

fmt.Println(title, "written by", writer, "drawn by", artist, "published by", publisher, year, "page", pageNumber, grade, "Grade")
}
```
What this prints out to is 
<p>
  Mr. GoToSleep written by Tracy Hatchet drawn by Jewel Tampson published by DizzyBooks Publishing Inc. 1997 page 14 6.5 Grade
</p>

## Additional coding

This code is an additional layer within the func main in Go. This shows how easy it is to compile multiple executions all in one package. 
```go
package main

import "fmt"

func main () {
  
var publisher, writer, artist, title string

title = "Mr. GoToSleep"
writer = "Tracy Hatchet"
artist = "Jewel Tampson"
publisher = "DizzyBooks Publishing Inc."

var year uint 
var pageNumber uint

year = 1997
pageNumber = 14

var grade float32

grade = 6.5

fmt.Println(title, "written by", writer, "drawn by", artist, "published by", publisher, year, "page", pageNumber, grade, "grade")

fmt.Println()

// Assigns will go here
title = "Epic Vol. 1"
writer = "Ryan N. Shawn"
artist = "Phoebe Paperclips"
publisher = "DizzyBooks Publishing Inc."
year = 2013
pageNumber = 160
grade = 9.0

fmt.Println(title, "written by", writer, "drawn by", artist, "published by", publisher, year, "page", pageNumber, grade, "grade")
}
```
This prints out
  ```
  Mr. GoToSleep written by Tracy Hatchet drawn by Jewel Tampson published by DizzyBooks Publishing Inc. 1997 page 14 6.5 grade

  Epic Vol. 1 written by Ryan N. Shawn drawn by Phoebe Paperclips published by DizzyBooks Publishing Inc. 2013 page 160 9 grade
```
</br>
As you can see you can build multiple executions all in one main function.  
