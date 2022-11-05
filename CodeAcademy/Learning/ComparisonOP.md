# Comparison OP

Logic Operators

| Operator | Meaning |
|----------|---------|
|     <    | Less than |
|     >    | Greater than |
|     <=   | Less than or equal to |
|     >=   | Great than or equal to | 

For example `100 < 200` is true. But if we use `100.5 <= 100.5` that is also true.

### Code Sample

Create an if statement that check if `vaultAmt` is at least $200,000 (200000) and print out line "We're going to need more bags."

```go
package main

import "fmt"

func main() {
	vaultAmt := 2356468
	
  // Add your code below:
  if vaultAmt >= 200000 {
    fmt.Println(" We're going to need more bags.")
  }
}
```
