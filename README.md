# Audit-Log-Pro

A structured audit logging library with compliance patterns for Python applications.

## Overview

Audit-Log-Pro provides enterprise-grade audit logging with structured events, retention policies, and compliance-ready formats.

## Features

- **Structured Events**: JSON-based audit entries with schema validation
- **Audit Context**: Automatic capture of actor, timestamp, and action metadata
- **Retention Policies**: Configurable log rotation and archival
- **Compliance Patterns**: SOC2, GDPR-ready event formats

## Installation

Install from source using uv:

```bash
uv pip install git+https://github.com/vindicta-platform/Audit-Log-Pro.git
```

Or clone and install locally:

```bash
git clone https://github.com/vindicta-platform/Audit-Log-Pro.git
cd Audit-Log-Pro
uv pip install -e .
```

## Quick Start

```python
from audit_log import AuditLogger

logger = AuditLogger(output="./audit.log")

logger.log(
    action="user.login",
    actor="user:alice",
    resource="session:12345",
    outcome="success"
)
```

## Related Repositories

| Repository | Relationship |
|------------|-------------|
| [platform-core](https://github.com/vindicta-platform/platform-core) | Parent platform |
| [Atomic-Ledger-Py](https://github.com/vindicta-platform/Atomic-Ledger-Py) | Financial audit trail |

## Platform Documentation

> **📌 Important:** All cross-cutting decisions, feature proposals, and platform-wide architecture documentation live in [**Platform-Docs**](https://github.com/vindicta-platform/Platform-Docs).
>
> Any decision affecting multiple repos **must** be recorded there before implementation.

- 📋 [Feature Proposals](https://github.com/vindicta-platform/Platform-Docs/tree/main/docs/proposals)
- 🏗️ [Architecture Decisions](https://github.com/vindicta-platform/Platform-Docs/tree/main/docs)
- 📖 [Contributing Guide](https://github.com/vindicta-platform/Platform-Docs/blob/main/CONTRIBUTING.md)

## License

MIT License - See [LICENSE](./LICENSE) for details.
