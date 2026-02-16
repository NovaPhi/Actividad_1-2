# Activity 1.1 - Regular languages
Version 2.0

Reference for math symbols:
https://www.overleaf.com/learn/latex/List_of_Greek_letters_and_math_symbols

VSCode plugin to view graphs:
**Markdown Preview Mermaid Support**
https://mermaid.js.org/syntax/flowchart.html

## Names:
- Luis Jaime Arias
- Pablo Sedano Morlett


## Exercises:

1. Give a recursive definition of the set of even natural numbers.

    _**SOLUTION:**_

    $S = \{2, 4, 6 , 8, 10, ... ,\N\}$
    
    **I. Basis:**
    $x = 2 \in S$ 

    **II. Recursive Step:**
    If $n \in S$, Then $n+2 \in S$

    **III. Closure:**
    $n \in S$ only if it can be obtained from the basis using a finite number of the recursive step


0. Prove by induction that $n^3 + 2n$ is divisible by 3 for all natural numbers $n$.

    _**SOLUTION:**_

    **I. Basis:**    
    If $n = 1$, Then $(n^3 + 2n) \: $%$ \: 3 = 0$ 

    
    $n = 1$

    $(1^3 +2(1) ) \: $%$ \: 3 = 0$

    **II. Inductive Hypothesis:**
    $n=k$

    $(k^3 + 2k) \: $%$ \: = 0 $
    
    **III. Inductive Step**
    $n = k+1$
    
    $((k+1)^3 + 2(k+1)) \: $%$ \: 3 = 0$
    
    $(k^3 + 3k^2 + 5k + 3) \: $%$ \: 3= 0$

    $((k^3 + 2k) + 3(k^2 + k + 1)) \: $%$ \: 3 =0$

    $n = 1$
    $3(1^3 + 1 + 1) \: $%$ \: 3$ = 0
    □


0. Prove by induction on $n$ that:

    $\sum_{i=0}^{n} 2^i = 2^{n + 1} - 1$

    _**SOLUTION:**_
    **I. Basis:**    
    if $n=0,$ then $2^{0+1}-1=1$

    **II. Inductive Hypothesis:**
    $n=k$
    $\sum_{i=0}^{k}2^i=2^{k+1}-1$
    
    **III. Inductive Step**
    $n=k+1$
    $\sum_{i=0}^{k+1}2^i=2^{(k+1)+1}-1$
    $\sum_{i=0}^{k}2^i+2^{k+1}=2^{(k+1)+1}-1$
    $2^{k+1}+2^{k+1}-1=2^{(k+1)+1}-1$
    $2^1\cdot2^{k+1}-1=2^{(k+1)+1}-1$
    $2^{(k+1)+1}-1=2^{(k+1)+1}-1$
    □


<!--
0. Using the tree below, give the values of each of the items:

    ```mermaid
    graph TD;
        x1-->x2;
        x1-->x3;
        x1-->x4;
        x2-->x5;
        x2-->x6;
        x2-->x7;
        x3-->x8;
        x3-->x9;
        x4-->x10;
        x5-->x12;
        x7-->x13;
        x7-->x14;
        x9-->x15;
        x9 -->x16;
        x10-->x17;
        x10-->x18;
        x13-->x19;
        x16-->x20;
    ```


    a. the depth of the tree

    `4`

    b. the ancestors of x18

    `x10, x4, x1`

    c. the internal nodes of the tree

    `x1, x2, x3, x4, x5, x7, x9, x10, x13, x16`

    d. the length of the path from x3 to x16

    `2`

    e. the vertex that is the parent of x13

    `x7`

    f. the vertices children of x10

    `x17, x18`

    --->