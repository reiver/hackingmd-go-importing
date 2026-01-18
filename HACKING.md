# HACKING: Importing in Golang

This `HACKINGS.md` document describes how to deal with **importing** in the **Go programming-lanuage** (**golang**).

-----

Imports have 3 groups.
For example:

```golang
import (
	"fmt"
	"io"

	"codeberg.org/reiver/go-erorr"
	"codeberg.org/reiver/go-log"
	"github.com/microcosm-cc/bluemonday"
	"github.com/yuin/goldmark"

	"example.com/joeblow/myprogram/cfg"
	"example.com/joeblow/myprogram/src/log"
)
```

(Note that in this _example_, `"example.com/joeblow/myprogram"` represents this _example_ program's _module name_.
In the actual source-code for this program, you would use this program's actual _module name_ — which is specified in this program's `go.mod` file.)

The **top group** in an `import` is for Go built-in packages.

The **bottom group** in an `import` is for packages in this program's source-code.

The **middle group** in an `import` is for _all other_ imports.
