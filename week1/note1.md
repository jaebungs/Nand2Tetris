# Boolean Functions and Gate Logic Roadmap
ohhh reminds me college electrical engineering class...
Since I know all the lgoic gates and how it works (experimented with chips, light bulbs, etc), I won't make all the logic gate.

## Boolean Logic

0       1
true    false
on      off

Ways to express Boolean Functions
Boolean Expression <=> Truth Table (Can convert both way)

f(x, y, z) = (x AND y) OR (NOT(x) AND z)
        ^
        |
        ⌄
x | y | z | f
0 | 0 | 0 | 0
0 | 0 | 1 | 1
    .
    .  
    .
Converting Boolean Expression to Truth Table is straight forward.
How about converting Truth Table to Boolea Expression?
First, focus on the result that is 1. Make expressions that gives 1 in the Truth Table.
Second, now we have bunch of different expressions. Do OR all the expressions.
Third, make it simpler/shorter/efficient.

De Morgan's Laws:
1. The complement of a conjunction (AND) is the disjunction (OR) of the complements:
NOT(x AND y) = NOT(x) OR NOT(y)

2. The complement of a disjunction (OR) is the conjunction (AND) of the complements:
NOT(x or y) = NOT(x) AND NOT(y)

#### NAND function (NOT(x AND y))
x | y | NAND
0 | 0 | 1
0 | 1 | 1
1 | 0 | 1
1 | 1 | 0


## Hardware Description Language (HDL)
I remember I really enjoyed this when I was in college.

Language that describes implementation of a chip. ex) OR(a=aAndnotb, b=notaAndb, out=out)
Interface is uniqude, but implementation is not. 

-VHDL
-Verilog
-Many more...

## Hardware Simulation
Helps verifing HDL program. Script based simulation, one file is HDL, the other is test file.

