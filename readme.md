# 🐍 Python Playground

**[https://h1jam.github.io/CodePlayground/](https://h1jam.github.io/CodePlayground/)**

A browser-based Python editor powered by [Pyodide](https://pyodide.org). No install, no server — runs entirely in your browser.

## Features

- **Code editor** with syntax highlighting, line numbers, and indent guides
- **Multi-file support** — create, rename, and delete `.py` files in the sidebar
- **Run Python** with `matplotlib`, `numpy`, and `requests` pre-loaded
- **Plot output** — `plt.show()` renders charts inline in the console
- **Virtual File System** — use `open()`, `os.mkdir()`, etc. as normal; files and folders appear in the VFS panel
  - Upload files from your machine into the virtual FS
  - Download any file produced by your code
  - Delete files or folders (recursive)
- **Export / Import** — save your entire workspace as a `.json` file and reload it later
- **Save** the active file as a `.py` download

## Usage

```python
import matplotlib.pyplot as plt
import numpy as np

x = np.linspace(0, 2 * np.pi, 100)
plt.plot(x, np.sin(x))
plt.show()
```

```python
import os

os.mkdir('output')
with open('output/result.txt', 'w') as f:
    f.write('Hello from Python!')
```

```python
import requests

r = requests.get('https://api.github.com')
print(r.status_code)
```

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+/` | Toggle comment |
