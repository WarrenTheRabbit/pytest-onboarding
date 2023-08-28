The `mark` package provides generic mechanisms for marking and selecting python functions.
It is located at `src/_pytest/mark`.

### Directory Structure
```
__init__.py
expression.py
structures.py
```
#### `__init__.py` structure
##### imports
```mermaid
flowchart LR
  __init__ --> dataclasses & typing & expression & structures & config & stash & nodes
  expression --> Expression & ParseError
  structures --> EMPTY_PARAMETERSET_OPTION & get_empty_parameterset_mark & Mark & MARK_GEN & MarkDecorator & MarkGenerator & ParameterSet
  config --> Config & ExitCode & hookimpl & UsageError & Parser
  stash --> StashKey
  nodes -- test invocation items --> Item
```






