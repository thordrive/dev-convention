[[_TOC_]]

## Imports
- Imports should be on separate lines.

  >**Bad**👎
  >```python
  >import os, sys
  >from module import func1, func2
  >```

  >**Good**👍
  >```python
  >import os
  >import sys
  >from module import (
  >    func1,
  >    func2
  >)
  >```