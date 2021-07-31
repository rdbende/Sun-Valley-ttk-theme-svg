# Sun-Valley-ttk-theme
A stunning theme for ttk based on Microsoft's Sun Valley visual style. This time with SVG images.

<br>

## Note
Light theme not available yet

## Documentation
For the documentation see the [documentation](DOCUMENTATION.pdf)!

## How to use?
I wanted to make usage of the theme very simple, so the theme setting is handled by a separate tcl script.
This way whether you want to use a dark or light theme, you need to import just a single file. The other thing
that makes this a good solution is that normally switching between light and dark theme is not entirely perfect,
and the colors doesn't change properly.

```python
import tkinter as tk
from tkinter import ttk

import tksvg

root = tk.Tk()
tksvg.load(root)

# Just simply import the sun_valley.tcl file
root.tk.call("source", "sun_valley.tcl")

# Then set the theme you want with the set_theme procedure
root.tk.call("set_theme", "dark")

root.mainloop()
```

## What's next?
Check out my other themes!
- [Azure ttk theme](https://github.com/rdbende/Azure-ttk-theme)
- [Forest ttk theme](https://github.com/rdbende/Forest-ttk-theme)
