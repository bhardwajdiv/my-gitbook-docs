# Navigation Hierarchy Setup

This section covers the underlying design architecture behind how nested sidebars are executed using Markdown configuration tracking.

## Nested Hierarchy Syntaxes
To transform a flat, single-tier list of loose documents into an elegant drop-down system, utilize standard double-space tab markers inside the indexing map file:

### Structural Schema Mapping Example
```markdown
* [Parent Documentation Node](parent.md)
  * [Child Component Sub-Node](folder/child.md)