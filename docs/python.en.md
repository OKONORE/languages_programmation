# 🐍 Python

## Definition

!!!note "Definition"
    Python is an interpreted, multi-paradigm, cross-platform programming language. It promotes structured, functional and object-oriented imperative programming. It has strong dynamic typing, automatic memory management by garbage collection and an exception handling system.
    __*source: Wikipedia[^wiki1]*__
    [^wiki1]: [Wikipedia : Definition](https://fr.wikipedia.org/wiki/Python_(langage))

- [X] Functional Oriented    
- [X] Object Oriented

!!!info "Information"
    We quickly introduce pyton in order to have a comparison with the languages that will be presented afterwards.

## Sample codes

### HelloWorld

- To begin, we will see how to write `helloworld` in the python console:

!!!Note "Write `helloworld`"

    === "Code 1"
        !!!Success "Success"
            ```python linenums="1"
            --8<-- "docs/scripts/python/helloworld/helloworld1.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/helloworld/helloworld1console.py"
            ```
            Here is how to write `helloworld` to the console. The `print` function is used to write to the console what it contains. Here it contains `"hello world"` which is a string.
            
    === "Code 2"
        !!!failure "Error"
            ```python linenums="1" hl_lines="1"
            --8<-- "docs/scripts/python/helloworld/helloworld2.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/helloworld/helloworld2console.py"
            ```
            Here the error is that the quotation marks were forgotten, and so, try to write the `hello` and `world` variable. Since these have not been defined, nothing comes out of the print and the program crashes.

    === "Code 3"
        !!!failure "Error"
            ```python linenums="1" hl_lines="1"
            --8<-- "docs/scripts/python/helloworld/helloworld3.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/helloworld/helloworld3console.py"
            ```
            Here the error is that the parentheses have been forgotten, and a function always has them, so the interpreter does not understand what this print does in front of a string.

### Loops
    
- Here we will see how to make a loop that sends the numbers from 0 to 10 inclusive to the console.

!!!Note "Loops"

    === "Code 1"
        !!!Success "Success"
            ```python linenums="1"
            --8<-- "docs/scripts/python/loops/boucle1.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/boucles/boucle1console.py"
            ```
            This is how a boucle is made in python. So it allows you to write in a 10 round boucle, numbers 0-11 excluded.
    
    === "Code 2"
        !!!Success "Success"
            ```python linenums="1"
            --8<-- "docs/scripts/python/boucles/boucle2.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/boucles/boucle2console.py"
            ```
            Here is a second way, less optimized, because if there are 1000 numbers, you have to write them all by hand, but it works.

    === "Code 3"
        !!!failure "Error"
            ```python linenums="1" hl_lines="2"
            --8<-- "docs/scripts/python/boucles/boucle3.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/boucles/boucle3console.py"
            ```
            Here the error is that the name of the variable in the loop is not the same as the one in the print, so the variable doesn't even exist.

### Mathematics

!!!note "Mathematics"
    python is also a tool to do mathematics, it can be sometimes simpler, to use python for repetitive formulas, in order to realize instantly the calculations.

- Here we will see how to transform this formula into a python code, which will return the result in the console

$$
\Delta = b^2-4ac
$$

> This formula is used to calculate Delta

!!!Note "Mathematics"

    === "Code 1"
        !!!Success "Success"
            ```python linenums="1"
            --8<-- "docs/scripts/python/delta/delta1.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/delta/delta1console.py"
            ```
            Here is the easiest way to calculate a Delta, to change the values, you will just have to change the values of "a", "b" and "c", or put an `int(input())` to ask the user of the script what values the user wants to perform the calculation.
    
    === "Code 2"
        !!!Success "Success"
            ```python linenums="1"
            --8<-- "docs/scripts/python/delta/delta2.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/delta/delta2console.py"
            ```
            Here is a second way to calculate Delta, but it is only valid for 1 calculation, otherwise you have to modify the elements in print. While the first one can quickly adapt with user inputs by changing the value of each variable.

    === "Code 3"
        !!!failure "Error"
            ```python linenums="1" hl_lines="2"
            --8<-- "docs/scripts/python/delta/delta3.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/delta/delta3console.py"
            ```
            Here the error is that the variables "a", "b" and "c" are not initialized, so the print cannot write the requested result.

### Lists

- Here we will see an example to send each element of a list to the console

!!!Note "Lists"

    === "Code 1"
        !!!Success "Success"
            ```python linenums="1"
            --8<-- "docs/scripts/python/listes/listes1.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/listes/listes1console.py"
            ```
            Here is how to send each element of a given list to the console.
    
    === "Code 2"
        !!!Success "Success"
            ```python linenums="1"
            --8<-- "docs/scripts/python/listes/listes2.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/listes/listes2console.py"
            ```
            Here the program also works, because the list is given directly in the for loop, without being in a variable, the code is less clear.

Now that we have seen the basics of python elements, we can compare them to lua
[💻 lua](lua.en.md){ .md-button }
