It is possible to include maths in Atomic Learning pages by using syntax which supports mathmode content.

# Inline Maths

To create inline maths in an Atomic Learning page, you can wrap the maths expression in dollar signs. For example, this sentence contains an inline maths expression: $x^2 + y^2 = z^2$. It is written in the source file as:

```markdown
This sentence contains an inline maths expression: $x^2 + y^2 = z^2$.
```

# Single Equations

To create a single equation, use a pair of double dollar signs. For example, the following is a single equation:

$$
x^2 + y^2 = z^2
$$

It was created wit the following source code:

```markdown
$$
x^2 + y^2 = z^2
$$
```

All equations are automatically numbered, and the number is displayed to the right of the equation.

## Equation Blocks

Equation blocks are used to display multiple equations together. This is achieved by using a pair of double dollar signs and separating each equation with a double backslash. For example, the following is an equation block:

$$
\begin{align}
x^2 + y^2 = z^2 \\
a^2 + b^2 = c^2
\end{align}
$$

This was created with the following source code:

```markdown
$$
\begin{align}
x^2 + y^2 = z^2 \\
a^2 + b^2 = c^2
\end{align}
$$
```

## Aligning Equations

To align entities within the align environment, you can use the ampersand (&) symbol. For example, the following is an aligned equation block:

$$
\begin{align}
0 &= &3x^2 &+ x &+ 1 \\
0 &= &x^2 &- 3x \\
0 &= &4x^2 & &+ 6
\end{align}
$$

This was created using the following source code:

```markdown
$$
\begin{align}
0 &= &3x^2 &+ x &+ 1 \\
0 &= &x^2 &- 3x \\
0 &= &4x^2 & &+ 6
\end{align}
$$
``` 

The character following the first ampersand in each equation is aligned with the character following the first ampersand in the other equations. The same applies to the second ampersand, and so on. It is not required that there is the same number of ampersands in each equation.

In practice, it is often good practice to align the equals signs in a set of equations, as this makes it easy to compare the left and right hand sides of each equation in a block.

# Referencing Equations in Text

You can give a label to an equation by using the `\label{}` command inside the equation environment. For example, the following equation has a label of `eq:pythagoras`:

$$
c^2 = a^2 + b^2 \label{eq:pythagoras}
$$

and was created with the following source code:

```markdown
$$
c^2 = a^2 + b^2 \label{eq:pythagoras}
$$
``` 

You can then reference this equation in the text using the `\ref{}` command. This sentence references Equation \ref{eq:pythagoras}. It was created with the following source code:

```markdown
This sentence references Equation \ref{eq:pythagoras}.
```
