/prompts/raw_data/create_import_diagram.md

#### CONTEXT
Each python file should have a mindmap that visualises its imports.
```mermaid
flowchart LR
    subgraph input
        a[.py file]
    end
    subgraph output
        b["mindmap of the modules
        used by the .py file"]
    end
    input --> output
```


#### INPUT
```python
#src/_pytest/cacheprovider.py
from .pathlib import resolve_from_str
from .pathlib import rm_rf
from .reports import CollectReport
from _pytest import nodes
from _pytest._io import TerminalWriter
from _pytest.config import Config
from _pytest.config import ExitCode
from _pytest.config import hookimpl
from _pytest.config.argparsing import Parser
from _pytest.deprecated import check_ispytest
from _pytest.fixtures import fixture
from _pytest.fixtures import FixtureRequest
from _pytest.main import Session
from _pytest.nodes import File
from _pytest.python import Package
from _pytest.reports import TestReport
```

#### OUTPUT
#### IMPORTS
|imports |source |
|--|---| 
|[pathlib](#pathlib)| [*/src/_pytest/pathlib.py*](https://github.com/pytest-dev/pytest/blob/main/src/_pytest/pathlib.py) |
|[reports](#reports)|[*/src/_pytest/reports.py*](https://github.com/pytest-dev/pytest/blob/main/src/_pytest/reports.py) |
|[_pytest](#_pytest)|[*/src/_pytest/*](https://github.com/pytest-dev/pytest/blob/main/src/_pytest)|
|[_pytest.config](#_pytestconfig)|[*/src/_pytest/config*](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/config)|
|[_pytest.config.argparsing](#_pytestconfigargparsing)|[*/src/_pytest/config/argparsing*](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/config/argparsing)|
|[_pytest.deprecated](#_pytestdeprecated)|[*/src/_pytest/deprecated*](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/deprecated)|
|[_pytest.fixtures](#_pytestfixtures)|[*/src/_pytest/fixtures.py*](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/fixtures.py)|
|[_pytest.main](#_pytestmain)|[*/src/_pytest/main.py*](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/main.py)|
|[_pytest.nodes](#_pytestnodes)|[*/src/_pytest/nodes.py*](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/nodes.py)|
|[_pytest.python](#_pytestpython)|[*/src/_pytest/python.py*](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/python.py)|
|[_pytest.reports](#_pytestreports)|[*/src/_pytest/reports.py*](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/reports.py)|
|[_pytest._io](#_pytestio)|[*/src/_pytest/io*](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/_io) |

<hr>
##### .pathlib
```mermaid
mindmap
    cacheprovider.py
        [resolve_from_str]
        [rm_rf]
```
[source](https://github.com/pytest-dev/pytest/blob/main/src/_pytest/pathlib.py.py) | [go back](#imports)

<hr>
##### .reports
```mermaid
mindmap
    cacheprovider.py
        [CollectReport]
```
[source](https://github.com/pytest-dev/pytest/blob/main/src/_pytest/reports.py.py) | [go back](#imports)

<hr>
##### _pytest
```mermaid
mindmap
    cacheprovider.py
        nodes
```
[source](https://github.com/pytest-dev/pytest/blob/main/src/_pytest/nodes.py) | [go back](#imports)

<hr>
##### _pytest.config
```mermaid
mindmap
    cacheprovider.py
        [Config]
        [ExitCode]
        [hookimpl]
```
[source](https://github.com/pytest-dev/pytest/blob/main/src/_pytest/config) | [go back](#imports)

<hr>
##### _pytest.config.argparsing
```mermaid
mindmap
    cacheprovider.py
        [Parser]
```
[source](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/config/argparsing.py) | [go back](#imports)

<hr>
##### _pytest.deprecated
```mermaid
mindmap
    cacheprovider.py
        [check_ispytest]
```
[source](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/deprecated.py) | [go back](#imports)

<hr>
##### _pytest.fixtures
```mermaid
mindmap
    cacheprovider.py
        [fixture]
        [FixtureRequest]
```
[source](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/fixtures.py) | [go back](#imports)

<hr>
##### _pytest.main
```mermaid
mindmap
    cacheprovider.py
        [Session]
```
[source](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/main.py) | [go back](#imports)

<hr>
##### _pytest.nodes
```mermaid
mindmap
    cacheprovider.py
        [File]
```
[source](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/nodes.py) | [go back](#imports)

<hr>
##### _pytest.python
```mermaid
mindmap
    cacheprovider.py
        [Package]
```
[source](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/python.py) | [go back](#imports)

<hr>
##### _pytest.reports
```mermaid
mindmap
    cacheprovider.py
        [TestReport]
```
[source](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/reports.py) | [go back](#imports)

<hr>
##### _pytest._io
```mermaid
mindmap
    cacheprovider.py
        [TerminalWriter]
```
[source](https://github.com/pytest-dev/pytest/tree/main/src/_pytest/_io) | [go back](#imports)