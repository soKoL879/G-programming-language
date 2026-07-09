# G-programming-language
This is my programming language I made myself, so excpect the compiler to be buggy on v1. it compiles to python so you need python installed too. When specifiyng the folder to compile to, please also specify the script name like C:\G\compiled.py. Aside from this, this is the documentation:                     



# G Programming Language v1.0

G compiles to Python. ; = block start. --- = block end.

## The 2 Rules
1. ; required at end of: func, if, elif, else, for, while
2. --- required to close EVERY block. One --- per block

## Examples

show("Hello G")
var x = 10

func greet(name);
show("Hello", name)
---
greet("world")

if x > 10;
show("big")
---
elif x > 5;
show("mid")
---
else;
show("small")
---

for i in range(5);
show(i)
---

var i = 0
while i < 3;
show(i)
var i = i + 1
---

func outer();
func inner();
show("nested")
---
show("outer")
---
outer()

break
continue

var name = input("Name? ")
show("Hi", name)

# Parcel
var p = Parcel()
p.append("first")
p.append("second")
show(p.join(", "))
