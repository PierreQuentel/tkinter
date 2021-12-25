Port of the GUI library tkinter for Brython.

The initial plan was to include it Brython standard distribution.

The adaptation of all tkinter widgets was either very difficult for some
widgets (eg Text), or impossible in the browser environment (blocking dialog
boxes).

For these reasons, the package is removed from Brython and created as a
distinct repository in case other developers wanted to resume its
development.

# Usage

Add this script in a Brython-enabled HTML page to run the current development
version:

```xml
<script src="https://raw.githack.com/PierreQuentel/tkinter/master/tkinter/tkinter.brython.js"></script>
```

# Generate tkinter.brython.js

Developers can generate this script with the CPython Brython package available with

```
pip install brython
```

Then, in a console window, navigate to the local repository in the subfolder
"tkinter" and run

```
brython-cli --make_package tkinter
```