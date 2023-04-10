---
published: false
---
How to merge two command class?

cd_fif4.py:
```py
class Command:
```

bottom_panel.py:
```py
class Command:
```

__init__.py:
```py
from .bottom_panel import * #
from .cd_fif4 import * #
```

result:
```py
AttributeError: 'Command' object has no attribute 'show_dlg'
ERROR: Exception in CudaText for cuda_find_in_filesX.show_dlg: AttributeError: 'Command' object has no attribute 'show_dlg'
```

cudatext.