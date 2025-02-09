# Fix Values with `Interact`

This guide addresses how to fix the value for certain arguments with Panel `interact`.

First, let's declare a simple function.

```{pyodide}
import panel as pn
from panel.interact import fixed
pn.extension() # for notebook

def f(x, y):
    return x, y
```

Now, call `interact` using the `panel.interact.fixed` function to fix one of the values:

```{pyodide}
pn.interact(f, x=1, y=fixed(10))
```

## Related Resources

- Read [Background > Widget Abbreviations for Panel Interact](../../background/interact/interact_abbreviations.md) for explanation.
- See [How-to > Autogenerate Widgets for Functions](../interact/index.md) for solutions.
- Consult [Reference > panel.interact] for technical details.
