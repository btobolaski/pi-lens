---
section: Fixed
---

- **Global inspection ignores (refs #703)**: Honor global `ignore` patterns for Git-tracked files, so excluding `**/*.yaml` and `**/*.yml` also disables automatic YAML inspection and yamllint. Invalidate existing graph snapshots so reports do not retain excluded files. Preserve `.gitignore` tracked-file handling and project negation overrides.
