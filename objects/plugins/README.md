#### What are plugins?

*Okken* writes: 
The `conftest.py` file is treated as a 'local plugin' and can contain hook functions and fixtures. 

```mermaid
graph LR
    subgraph plugin
        hook[hook functions]
        fixtures
    end
```

#### How do plugins relate to other objects?

```mermaid
graph LR
    plugin
    hook[hook function]
    fixture
    
```

#### Example Plugins
| name | source | access | summary|
| --- | --- | --- | ---- |
| cacheprovider | private | ? |

