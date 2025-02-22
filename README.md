# martypy

Python library to communicate with Marty the Robot V1 and V2 by Robotical

[See the API Documentation](https://userguides.robotical.io/martyv2/documentation/python_function_reference)

To regenerate documentation:
- pip install -r dev-requirements.txt
- pydoc-markdown --server --open

## How to run example scripts

If you cloned the repository or downloaded the source code to try the [example scripts](examples),
you will need to make sure you have MartyPy installed before you can run the examples.

The easiest way to install MartyPy is with the `pip install martypy` script as explained in
[step 2 here](https://userguides.robotical.io/martyv2/userguides/python/setting_up_python_on_your_computer).

If you would like to make modifications to the martypy library itself, it will be better to install
it from source using the command `pip install --editable /path/to/martypy/repo` (replacing
`/path/to/martypy/repo` as appropriate of course).

If you do not want to "`pip install`" the MartyPy library, you can add the following 4 lines at the
top (before any other code) of each script you want to run:

```python
import sys
import pathlib
cur_path = pathlib.Path(__file__).parent.resolve()
sys.path.append(str(cur_path.parent.resolve()))
```
