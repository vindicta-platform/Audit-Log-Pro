# Getting Started

```bash
uv pip install git+https://github.com/vindicta-platform/Audit-Log-Pro.git
```

```python
from audit_log import Logger

logger = Logger()
logger.log("CREDIT_CONSUMED", amount=10, user="user-1")
```
