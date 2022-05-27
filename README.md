# textwrap

Based on Python textwrap module.

## Usage / example

```go
package main

import (
	"fmt"
	"github.com/marhar/textwrap"
)

func main() {
	s := `
		Lorem ipsum dolor sit amet,
		consectetur adipiscing elit.
		Curabitur justo tellus, facilisis nec efficitur dictum,
		fermentum vitae ligula. Sed eu convallis sapien.`
	fmt.Println("-------------")
	fmt.Println(s)
	fmt.Println("-------------")
	fmt.Println(textwrap.Dedent(s))
}
```

```bash
$ go run main.go
-------------
Lorem ipsum dolor sit amet,
consectetur adipiscing elit.
Curabitur justo tellus, facilisis nec efficitur dictum,
fermentum vitae ligula. Sed eu convallis sapien.
-------------
		Lorem ipsum dolor sit amet,
		consectetur adipiscing elit.
		Curabitur justo tellus, facilisis nec efficitur dictum,
		fermentum vitae ligula. Sed eu convallis sapien.
```

## Acknowledgements

Dedent copied from github.com/lithammer/dedent.


## License

MIT
