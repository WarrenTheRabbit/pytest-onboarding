#### Debugging with VS Code
To debug the *pytest* package in VS Code, you will need to [configure its debugger](https://code.visualstudio.com/docs/python/debugging#_initialize-configurations).
If you attempt to debug *pytest* as if it were a script, you will encounter import errors. 
To ensure modules are loaded correctly, add the following to the `launch.json` file:


##### Debugger Configuration
```json
{
  "version": "0.2.0",
  "configurations": [
    {
      "name": "Python: pytest",
      "type": "python",
      "request": "launch",
      "module": "pytest",
      "justMyCode": true
    },
  ]
}
```

#### When you don't use a configuration
For example, if you attempt to debug `src/_pytest/config/__init__.py` without a configuration and rely instead on the default 
behaviour of launching a debug session on an individual Python file, you would get the error:
![image](https://github.com/WarrenTheRabbit/case-studies/assets/37808734/980a52ef-1f51-4c74-87d2-f700197c26ab)

#### When you use a correct configuration
Instead, you need to configure the debugger to run *pytest* as a package and add breakpoints to locations of interest.
For example, if you add a breakpoint to line 47 of `src/_pytest/config/__init__.py` and launch the debugger session with 
[a pytest configuration](#####Debugger-Configuration), you can start debugging:
![image](https://github.com/WarrenTheRabbit/case-studies/assets/37808734/f3863fe3-40e1-4851-9831-3997b072648c)



