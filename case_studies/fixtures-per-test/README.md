| Issue                                                       | Date       | Author                                          | Summary                                                                     |
| ----------------------------------------------------------- | ---------- | ----------------------------------------------- | --------------------------------------------------------------------------- |
| [#11295](https://github.com/pytest-dev/pytest/issues/11295) | 2023-08-07 | [The-Compiler](https://github.com/The-Compiler) | `--fixtures-per-test` should exclude parametrizing fixtures from its output |

### Problem Statement



### First Steps

##### Create the example.

```python
#testing/learning_tests/test_file_that_will_create_example_behaviour.py

import pytest

def test_one(monkeypatch):
    pass

@pytest.mark.parametrize("x", [1, 2])
def test_two(x):
    pass

```

##### Open `launch.json`.

![VS Code Open 'launch.json` command](/media/open_launch_json.png)

```jsonc
{
  // Use IntelliSense to learn about possible attributes.
  // Hover to view descriptions of existing attributes.
  // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
  "version": "0.2.0",
  "configurations": [
    {
      // Existing Configuration 1 (if there is one)
    },
    {
      // Any existing Configuration 2 (if there is one)
    },
    {
      // etc
    }
  ]
}
```

#### Add a configuration
Updating `launch.json` will make it possible to debug _pytest_ as it executes the command 
```bash
pytest --fixtures-per-test ./testing/learning_tests/test_file_that_will_create_example_behaviour.py
```

```jsonc
{
  // Remove or include the message about IntelliSense.
  "version": "0.2.0",
  "configurations": [
    {
      // Existing configurations, if any.
    },
    {
      // The configuration that will be used
      // to learn more about the behaviour
      // we are seeking to change.
      "name": "Python: exclude-paramaterized",
      "type": "python",
      "request": "launch",
      "module": "pytest",
      "justMyCode": true,
      "args": [
        "--fixtures-per-test",
        ".\\testing\\learning_tests\\test_file_that_will_create_example_behaviour.py"
      ]
    }
  ]
}
```
#### Add a breakpoint
Without a breakpoint, the debugger will run from start to finish without an opportunity to inspect the execution context. 

We don't know where we want to add the breakpoints at this point. But we have some clues. 

| Clue | Reason | 
| --- | --- |
| `get_direct_param_fixture_func`  |  The-Compiler: "It doesn't make sense to show it as a fixture without a docstring which is "defined" here"   | 
| `--fixtures-per-test` | 