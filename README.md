This is a sample project to illustrate relative imports in python.

To run runner.py use the command
./runner.py
or
python3 runner.py
standing on the root of the project, if you would call it from other location, you have add the project directory to the PYTHONPATH environment variable.

If you want test relative_imports/b/b.py, use the
python3 -m relative_imports.b.b
command, ensuring that python finds the package.

Note:

if you run b.py as the module b.b e.g.
python3 -m b.b
the interpreter considers b to be the root package, and cannot resolve the relative import "from ..a.a import ..."

References:
- https://docs.python.org/3/reference/import.html
- https://www.python.org/dev/peps/pep-0328/
