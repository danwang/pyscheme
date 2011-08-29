# Pyscheme

A Scheme interpreter written in Python.

## Running the interpreter
### Normal mode

```
python pyscheme.py
```
### Debugging mode
Uses normal Python handling of exceptions

```
python pyscheme.py -d
```

In normal mode, Python exceptions are ignored and "Internal Error" is printed. With debugging mode, the familiar (Python) stacktrace is printed.

### Exiting the interpreter
Running the primitive ```(exit)``` will exit as a PyScheme routine. Additionally, the signals ```Ctrl+C``` and ```Ctrl+D``` (End of File) also halt PyScheme.

## Meta-Options
### Pretty-print
To turn pretty-print of numbers on and off, set the variable
```pretty-print```
(default is```#f```)

Example:

```
pyscheme > (define pretty-print #t)
okay
pyscheme > 1000
1,000
```
