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

### Aligning Equations

To align entities within the align environment, you can use the ampersand (&) symbol. For example, the following is an aligned equation block:

$$
\begin{align}
0 &= 3&x^2 + &x + &1 \\
0 &= &x^2 - 3&x \\
0 &= 4&x^2 & + &6
\end{align}
$$