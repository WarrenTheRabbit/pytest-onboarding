`[test link](https://github.com/pytest-dev/pytest/issues/11295)`

[test link](https://github.com/pytest-dev/pytest/issues/11295)

```mermaid
graph LR
a --> b
```

> [!NOTE]
> Highlights information that users should take into account, even when skimming.

> [!IMPORTANT]
> Crucial information necessary for users to succeed.

> [!WARNING]
> Critical content demanding immediate user attention due to potential risks.

#### Initial Exploration

##### Entry Point
```mermaid
sequenceDiagram
  participant Terminal as Terminal
  participant __main__ as __main__
  participant console_main as console_main
  participant main as main

  Terminal ->> __main__: pytest --fixtures-per-test
  __main__ ->> console_main: call
  console_main ->> main: call
  main ->> console_main: return code
  console_main ->> __main__: return code
```

##### Linkable Class Diagram with tooltips

```mermaid
classDiagram
class ClickHref
class ClickHrefSelfTarget
class ClickHrefTopTarget
class ClickHrefParentTarget

click ClickHref href "https://github.com/WarrenTheRabbit/pytest-onboarding/blob/main/objects/File/README.md" "This is a tooltip for a link"
click ClickHrefSelfTarget href "https://github.com/WarrenTheRabbit/pytest-onboarding/blob/main/objects/File/README.md" "This is a tooltip for a link" _self
click ClickHrefTopTarget href "https://github.com/WarrenTheRabbit/pytest-onboarding/blob/main/objects/File/README.md" "This is a tooltip for a link" _top
click ClickHrefParentTarget href "https://github.com/WarrenTheRabbit/pytest-onboarding/blob/main/objects/File/README.md" "This is a tooltip for a link" _parent
```
