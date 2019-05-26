# Header 1

## Header 2

### Header 3

#### Header 4

##### Header 5

###### Header 6

This is a test file for Typora. My theme is named “rain” because of my favourite perfume Rain under the brand Clean.

1. ordered-list

* unordered-list

> A test of the block quote

This is the *italic font*.

This is the **bold font**. 

<u>Underline looks like this</u>.

~~Deletion looks likes this.~~

This is a sample for ^sup^ and ~sub~.

==Highlight information==

inline `code`

inline $\textrm{math font } v=\hbar c$

Welcome to my Github repository [Siren-Blue/Rain](<https://github.com/Siren-Blue/Rain> )

| Table     |           |
| --------- | --------- |
| Odd line  | Odd line  |
| Even line | Even line |

````python
import matplotlib.pyplot as plt
from matplotlib.ticker import FuncFormatter as FF
import numpy as np  
import math

def problem1():
    E_g0 = 1.170 # eV
    alpha = 4.73 * 0.0001 # eV/K
    beta = float(636) # K
    E_g = []
    for T in range(600):
        T = float(T)
        E_g.append(E_g0 - (alpha * T * T) / (beta + T))
    plt.plot(range(600), E_g)
    plt.scatter(300, E_g[300], marker='o')
    plt.plot([300,300],[1,E_g[300]], linestyle="--")
    plt.plot([0,300], [E_g[300], E_g[300]], linestyle="--")
    plt.text(320, E_g[300], '(300, 1.125)')
    plt.xlabel('Temperature T (K)')
    plt.ylabel('Bandgap Energy E_g (J)')
    plt.xlim((0, 600))
    plt.ylim((1, 1.175))
    plt.savefig('p1.png')
    
````



